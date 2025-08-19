# Compiler Projects — Meta Repository

A curated hub of my compilers and tooling work: IR experiments, parsers, optimizers, and runtime explorations. One link for everything.

> 📌 Portfolio link target — share this repo URL in your Projects section.

---

## Highlights
- 🧱 **Front‑ends**: lexers/parsers (hand-rolled + generator-based)
- 🧠 **IR & Opt**: SSA, CSE/DCE, inlining, constant folding, loop opts
- ⚙️ **Back‑ends**: bytecode + native codegen experiments
- 🧪 **Tooling**: fuzzers, test harnesses, disassemblers, profilers

---

## Projects (Quick Table)

| Project | What it is | Key Tech | Repo |
|---|---|---|---|
| **ToyLang** | A small teaching compiler from AST → SSA IR → bytecode VM | C++17, ANTLR, SSA, bytecode | https://github.com/yourname/toylang |
| **MiniC** | C subset compiler with CFG + classic optimizations | LLVM passes, CFG, DCE, CSE | https://github.com/yourname/minic |
| **XIR** | Standalone IR playground + optimizer suite | Rust, arena allocators, SSA | https://github.com/yourname/xir |
| **RegAlloc Lab** | Interference graphs & coloring allocators | Rust, graph coloring | https://github.com/yourname/regalloc-lab |
| **WASM Toy** | High-level → Wasm + simple runtime | Wasm, WAT/wasmtime | https://github.com/yourname/wasm-toy |

> Tip: Keep this table tight—most reviewers scan here first.

---

## Deep Dives

### 1) ToyLang
- **Pipeline**: `lexer → parser → AST → SSA IR → regalloc → bytecode`
- **Notables**: constant folding, dead code elim, basic inliner  
- **Docs**: [/docs/toylang.md](./docs/toylang.md) (in that repo)

### 2) MiniC
- **Pipeline**: `C subset → CFG → LLVM IR → passes`  
- **Notables**: loop‑invariant code motion, GVN, simple SROA  
- **Docs**: see the `README` in repo

*(Add similar short sections for each.)*

---

## Demos
- ▶️ Short clips / asciinema links / screenshots if you have them.

---

## How to Explore
- Prefer **per-repo READMEs** for building/running specifics.
- Typical build pattern:
  ```bash
  # example
  cd toylang && mkdir -p build && cd build
  cmake .. && make -j
  ./toylang ../examples/hello.tl
