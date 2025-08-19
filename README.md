# Compiler Projects — Meta Repository

A curated hub of my compilers and tooling work: front-ends, IR transformations, optimizations, and back-end experiments.  
Built through the **UPenn Compilers course** and by recreating a **C-like compiler** from the *Making Compilers* book.

---

## Highlights
- 🧱 **Front-ends**: lexers/parsers (hand-rolled + generator-based)
- 🧠 **IR & Optimizations**: SSA, CSE/DCE, inlining, constant folding, loop opts
- ⚙️ **Back-ends**: bytecode, LLVM IR, WebAssembly
- 🧪 **Tooling**: test harnesses, debuggers, small runtimes

---

## Projects (Quick Table)

| Project | What it is | Key Tech | Repo |
|---|---|---|---|
| **x86lite** | Course project: subset of x86 compiler targeting a bytecode VM; covers lexing → parsing → IR → codegen | C++17, hand-rolled parser, SSA, bytecode VM | https://github.com/yourname/x86lite |
| **llvm-lite** | Course project: C-subset compiler lowering into LLVM IR with classic optimizations | LLVM passes, CFG, SSA, DCE, CSE | https://github.com/yourname/llvm-lite |
| **Type-Checked Compiler** | Extended compiler with semantic analysis + type checker; supports richer language features | Recursive-descent parsing, type system, IR checks | https://github.com/yourname/type-checked-compiler |
| **Recreated C** | A C-like compiler built from *Making Compilers*; end-to-end from lexing to executable/runtime | C++/Rust (specify yours), parser, type checker, codegen, simple runtime | https://github.com/yourname/recreated-c |

---

## 📸 Screenshots & Visuals

### x86lite
<p align="center">
  <img src="images/x86lite_ir.png" alt="IR dump example" width="600"/>
</p>
*IR dump showing SSA form before and after constant folding.*

---

### llvm-lite
<p align="center">
  <img src="images/llvm_cfg.png" alt="CFG graph" width="600"/>
</p>
*CFG generated from a sample function, used for data-flow optimizations.*

---

### Type-Checked Compiler
<p align="center">
  <img src="images/type_errors.png" alt="Type checker error reporting" width="600"/>
</p>
*Example of semantic/type errors caught during compilation.*
