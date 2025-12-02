<div align="center">
  
<!-- Sia Banner Logo -->
<svg width="600" height="160">
  <rect width="100%" height="100%" rx="18" fill="#0b63ce"/>
  <text x="50%" y="50%" dominant-baseline="middle" text-anchor="middle"
        font-size="48" font-family="Segoe UI, sans-serif" fill="white"
        font-weight="600">
    Sia Programming Language
  </text>
  <text x="50%" y="78%" dominant-baseline="middle" text-anchor="middle"
        font-size="20" font-family="Segoe UI, sans-serif" fill="#e8f1ff">
    A Lightweight Educational Compiler (Flex + Bison + C Backend)
  </text>
</svg>

</div>

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
Sia is a small, Python-inspired educational programming language built to demonstrate key compiler phases using **Flex**, **Bison**, and **C**.  
It features a clean syntax, automatic type inference, structured control flow, and a minimal backend that generates valid C code.  
(Reference: Sia User Manual)

---

# ✨ Core Features
- **Variables & Types:** INT, FLOAT, STR, Boolean with type inference  
- **Expressions:** arithmetic (+ − * /), relational operators, parentheses  
- **Control Flow:** `IF/ELSE`, `WHILE`  
- **I/O:** `GET var;`, `SHOW expr;`  
- **Compiler Pipeline:** Flex lexer → Bison parser → semantic checks → C code generation  

---

# ⚙️ Getting Started
### Prerequisites  
`flex`, `bison`, `gcc/clang`

### Build Steps
```bash
flex -o lex.yy.c src/sia.l
bison -d -o src/sia.tab.c src/sia.y
gcc -Iinclude src/*.c lex.yy.c src/sia.tab.c -o sia_compiler -lm


### Run a Program
```bash
./sia_compiler program.sia

