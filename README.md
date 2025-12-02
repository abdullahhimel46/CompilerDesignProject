# CompilerDesignProject — Sia

Sia is a lightweight, educational programming language designed to demonstrate the core phases of compiler construction (lexing, parsing, semantic analysis, and code generation) using Flex, Bison, and a C-based backend.  
The language features a clean, Python-like syntax and is intended for teaching and experimentation.

---

## 👥 Meet our team

<div style="display:flex; flex-wrap:wrap; gap:10px;">

<div style="background:#e8f1ff; padding:8px 12px; border-radius:8px;">Md Abdullah Himel — 1622</div>
<div style="background:#e8f1ff; padding:8px 12px; border-radius:8px;">Md Labib Ahmed Leo — 1147</div>
<div style="background:#e8f1ff; padding:8px 12px; border-radius:8px;">Zabir Bin Abu Bakar — 4752</div>
<div style="background:#e8f1ff; padding:8px 12px; border-radius:8px;">Poritos Das — 1736</div>
<div style="background:#e8f1ff; padding:8px 12px; border-radius:8px;">Mysha Milon Ohana — 1039</div>

</div>

---

## 📘 Project Overview

Sia demonstrates a full, simple compiler pipeline with readable internals and educational comments.

### Goals
- Teach lexical analysis with **Flex**
- Show grammar design and parsing with **Bison**
- Build a small AST and perform semantic checks
- Generate **C-based output** to illustrate backend compilation

---

## ✨ Features

- Python-like syntax  
- Tokenization & lexical rules with **Flex**  
- LR parsing using **Bison**  
- Semantic analysis (type checking, symbol table)  
- Simple **C backend** for code generation  

---

## ⚙️ Getting Started

**Prerequisites:** `flex`, `bison`, `gcc` / `clang`, `make`

### Build Example

```bash
# generate scanner & parser
flex -o lex.yy.c src/sia.l
bison -d -o src/sia.tab.c src/sia.y

# compile
gcc -Iinclude src/*.c lex.yy.c src/sia.tab.c -o sia_compiler -lm

# run
./sia_compiler examples/hello.sia
