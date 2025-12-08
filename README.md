<p align="center">
  <img src="assets/sia_banner.svg" width="720"/>
</p>

---

# 👥 Team Members
<div style="display:flex; flex-wrap:wrap; gap:10px;">

<div style="background:#e8f1ff; padding:8px 12px; border-radius:8px;">Md Abdullah Himel — 1622</div>
<div style="background:#e8f1ff; padding:8px 12px; border-radius:8px;">Md Labib Ahmed Leo — 1147</div>
<div style="background:#e8f1ff; padding:8px 12px; border-radius:8px;">Zabir Bin Abu Bakar — 4752</div>
<div style="background:#e8f1ff; padding:8px 12px; border-radius:8px;">Poritos Das — 1736</div>
<div style="background:#e8f1ff; padding:8px 12px; border-radius:8px;">Mysha Milon Ohana — 1039</div>

</div>

---

# 📘 Overview
Sia -> Simple, Interpretable, Analyzer  <br>
**Sia** (Syntax Interpreter & Analyzer) is a small, Python-inspired educational programming language created to illustrate every fundamental stage of compiler construction using:

- **Flex** — lexical analysis  
- **Bison** — parsing  
- **C backend** — code generation  

Sia supports a simple imperative structure, type inference, clean expressions, and essential control flow constructs, making it ideal for learning compiler design principles.

---

# ✨ Core Features
- **Primitive Types:** INT, FLOAT, STR, Boolean  
- **Type System:** explicit typing + automatic type inference  
- **Expressions:** +, −, *, /, relational ops, parentheses  
- **Control Flow:** `IF/ELSE`, `WHILE`  
- **I/O:** `GET var;`, `SHOW expr;`  
- **Full Compiler Pipeline:**  
  Flex → Bison → AST → Semantic Analysis → C Code Generation  

---

# ⚙️ Getting Started

### Prerequisites
Install the following:

- `flex`
- `bison`
- `gcc` or `clang`
- `Python 3.x`

### How to run a SIA program
--- For windows ---
```bash
.\sia_compiler.exe studentMarksCalc.sia
gcc studentMarksCalc.c -o studentMarksCalc.exe
.\studentMarksCalc.exe
```

### Or, use the batch file (one command)
```bash
.\run_sia.bat studentMarksCalc.sia
```


--- For Linux/Mac ---
```bash
# Build the Compiler
make

# Make Run script executable
chmod +x run_sia.sh

# Run the program
./run_sia.sh studentMarksCalc.sia
```

# Using makefile 
```bash
make run
FILE=studentMarksCalc.sia
```
