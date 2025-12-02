<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>CompilerDesignProject — Sia</title>
  <style>
    body { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial; line-height:1.6; color:#222; padding:24px; background:#f7fafc; }
    .container { max-width:900px; margin:0 auto; background:#fff; padding:28px; border-radius:10px; box-shadow:0 6px 18px rgba(20,20,30,0.06); }
    header h1 { margin:0 0 8px 0; color:#0b63ce; }
    header p.lead { margin:0 0 18px 0; color:#374151; }
    .team { display:flex; flex-wrap:wrap; gap:12px; margin:14px 0; }
    .member { background:#f1f8ff; padding:10px 14px; border-radius:8px; color:#0b63ce; font-weight:600; }
    section { margin-top:20px; }
    h2 { color:#0b63ce; margin-bottom:10px; }
    ul { margin:0; padding-left:20px; }
    pre { background:#0f1724; color:#e6eef8; padding:12px; border-radius:8px; overflow:auto; }
    footer { margin-top:28px; font-size:0.95rem; color:#6b7280; }
    .muted { color:#6b7280; font-size:0.95rem; }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>CompilerDesignProject — Sia</h1>
      <p class="lead">Sia is a lightweight, educational programming language designed to demonstrate the core phases of compiler construction (lexing, parsing, semantic analysis, and code generation) using Flex, Bison, and a C-based backend. The language features a clean, Python-like syntax and is intended for teaching and experimentation.</p>
    </header>

    <section>
      <h2>Meet our team</h2>
      <div class="team" aria-label="Team members">
        <div class="member">Md Abdullah Himel — 1622</div>
        <div class="member">Md Labib Ahmed Leo — 1147</div>
        <div class="member">Zabir Bin Abu Bakar — 4752</div>
        <div class="member">Poritos Das — 1736</div>
        <div class="member">Mysha Milon Ohana — 1039</div>
      </div>
    </section>

    <section>
      <h2>Project overview</h2>
      <p>Sia demonstrates a full, simple compiler pipeline with readable internals and educational comments. The main goals are:</p>
      <ul>
        <li>Teach lexical analysis with Flex</li>
        <li>Show grammar design and parsing with Bison</li>
        <li>Build a small AST and perform semantic checks</li>
        <li>Generate C-based output (or direct C code) to illustrate backend compilation</li>
      </ul>
    </section>

    <section>
      <h2>Features</h2>
      <ul>
        <li>Python-like syntax for ease of reading</li>
        <li>Tokenization & lexical rules with Flex</li>
        <li>LR-style parsing with Bison</li>
        <li>Semantic analysis (type checks, symbol table)</li>
        <li>Simple C backend demonstrating code generation</li>
      </ul>
    </section>

    <section>
      <h2>Getting started</h2>
      <p class="muted">Prerequisites: flex, bison, gcc (or clang), make</p>
      <p>Typical build steps (example):</p>
      <pre>
# generate scanner & parser
flex -o lex.yy.c src/sia.l
bison -d -o src/sia.tab.c src/sia.y

# compile
gcc -Iinclude src/*.c lex.yy.c src/sia.tab.c -o sia_compiler -lm

# run
./sia_compiler examples/hello.sia
      </pre>
      <p>Notes: adjust paths to your project layout. The commands above are illustrative.</p>
    </section>

    <section>
      <h2>Usage</h2>
      <p>Feed a .sia source file to the compiled compiler; it will run the pipeline and produce generated C or an executable depending on the chosen backend. See the <code>examples/</code> directory for sample programs.</p>
    </section>

    <section>
      <h2>Contributing</h2>
      <p>Contributions are welcome! Please open issues for bugs or feature requests and submit PRs for fixes or enhancements. Keep changes small and document any grammar or semantic changes.</p>
    </section>

    <footer>
      <p>Made with curiosity and a sprinkle of compiler magic ✨</p>
      <p class="muted">If you'd like, I can push this HTML-formatted README back to the repository for you — just confirm and I'll commit it, cutie 😉</p>
    </footer>
  </div>
</body>
</html>