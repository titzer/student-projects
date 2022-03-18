# Student projects

In this repo, you will find an up-to-date list of projects of various sizes and difficulties for students interested in working with me on class, research, or honors projects.
Some projects have a larger component of research (i.e. high novelty, many unknowns) than others.

## Research Projects

These projects have significant number of unknowns and design choices to make.
They represent more research-oriented topics with potential publication opportunities.

### [Packing ADTs](PackingADTs.md) - Virgil, moderate difficulty, high novelty

In this project, you will explore new techniques to represent algebraic data types (ADTs) more efficiently.
You will work on the internals of a sophisticated, static compiler for the Virgil programming language and introduce new analysis and optimizations in this compiler.
IMPACT: You will make Virgil completely outclass all languages to date and very likely publish a paper.
Compiler experience and some familiarity with functional programming required.

### [Design a Data Layout Embedded DSL for Virgil](DataLayouts.md) - Virgil, moderate difficulty, high novelty

In this project, you will design and implement new language constructs for describing memory layouts of fixed data structures such as network packets, kernel buffers, etc.
You will work on the internals of a sophisticated, static compiler for the Virgil programming language and introduce new analysis and optimizations in this compiler.
IMPACT: You will make Virgil the language of choice for low-level programming where memory layouts are fixed and likely publish a paper.
Compiler experience required.

### [Partial Specialization](PartialSpecialization.md) - Virgil, moderate difficulty, high novelty

In this project, you will explore new ways to implement polymorphic types.
You will work on the internals of a sophisticated, static compiler for the Virgil programming language and introduce new analysis and optimizations in this compiler.
You will investigate sharing polymorphic specializations before specialized code is generated.
IMPACT: You will make Virgil obliterate other languages with polymorphic types and very likely publish a paper.
Compiler experience and some programming language theory required.

### [Benchmark WebAssembly](BenchmarkWasm.md) - WebAssembly, fair difficulty, fair novelty

In this project, you will scour the planet for benchmarks for WebAssembly, creating a suite of freely-available kernels, micro-benchmarks, programs, and applications that is useful for studying all aspects of Wasm performance.
You will follow best practices from benchmarking literature and known suites such as SPEC and DaCapo and create a framework for easily obtaining statistically reliable, reproducible results.
IMPACT: You will make it easy to reliably benchmark any aspect of any Wasm engine and maybe publish the go-to paper on doing so.
Basic programming and scripting experience required, some familiarity with statistics.

### [MMTk for Virgil](MMTkVirgil.md) - Virgil, Rust, moderate difficulty, moderate novelty

In this project, you will aim to improve Virgil's garbage collection performance by interfacing with MMTk, a modern, high-performance, VM-agnostic GC framework.
You will work out how to interface the MMTk runtime with Virgil's runtime and develop necessary compiler modifications for the interoperability.
IMPACT: You will make Virgil GC state-of-the-art and maybe publish a paper.
Compiler experience and some familiarity with GC required.

### [Graph Coloring Register Allocator](RegAlloc.md) - Virgil, high difficulty, moderate novelty

In this project, you will write a new, sophisticated register allocator for the advanced Virgil compiler.
Despite being studied for five decades, register allocation remains a challenging problem.
You will explore new techniques to make graph coloring register allocation more efficient, in particular better
splitting heuristics and incremental rebuilding of the interference graph.
IMPACT: You will make Virgil run much faster and maybe publish a paper.
Compiler experience required.


## Feature Projects

Both Virgil (the programming language) and Wizard (the WebAssembly engine) can benefit from new features.
Adding new features to the Virgil programming language not only makes writing code more fun and expressive, but can enable new types of expression patterns and accompanying compiler optimizations that make VM development a whole lot nicer.
In particular, the Wizard engine should stay up-to-date with coming proposals, but also support platform features (like WASI) that make it possible to experiment with large, real programs.

### [Implement `wasi_snapshot_preview1` in Wizard on `x86-64-linux`](WasiWizard.md) - Virgil, low difficulty, low novelty, high priority

In this project, you will implement the WebAssembly System Interface (WASI) in the Wizard Engine.
You'll write code to interface directly with the Linux kernel to provide the lowest-overhead, no-dependency implementation of this interface.
IMPACT: You will greatly improve the number of applications Wizard can run, allowing testing, benchmarking, and studying full applications in direct comparison to production engines.
WebAssembly experience required, low-level system call familiarity required.

### [Integrate Virgil and Rust](WasiWizard.md) - Virgil/Rust, medium difficulty, high novelty, low priority

In this project, you will explore ways to make Virgil code interact with Rust.
A project with many unknowns, you will investigate different linking strategies (e.g. does the Virgil compiler generate an object file linked into a Rust executable or vice versa? what about dynamic linking?).
You might have to tinker with Virgil's startup routines and how it manages its heap.
You'll work on both the Virgil compiler and LLVM in order to develop a working solution.
IMPACT: You will greatly increase the number of places that Virgil can run and make it possible to use libraries written in Rust.
Some compiler experience required, familiarity with LLVM highly recommended.

## Porting Projects

Porting Virgil (the programming language) and Wizard (the research WebAssembly engine) to new plaforms opens up new possibilities.
For one, it makes development on new platforms more ergonomic and efficient, and secondly it overall increases the capabilities of both systems.
For Wizard to run on a platform natively, Virgil must first be ported.

### [Port Wizard's Fast Interpreter to JSC](PortWizardJSC.md) - C++, WebAssembly, high difficulty, moderate novelty

In this project, you will port (or rewrite) Wizard's fast in-place interpreter, hand-written in assembly, to JavaScriptCore.
You will add a new (or adapt the existing) interpreter tier which does not rewrite Wasm, but uses the original bytes.
IMPACT: You will demonstrate that WebAssembly can be interpreted in-place fast in a production engine and maybe publish a paper.
Assembly and C++ experience required.

### [Port Virgil to x86-64-darwin](PortVirgilX8664Darwin.md) - Virgil, low difficulty, low novelty, high priority

In this project, you will port Virgil to the `x86-64-darwin` platform, i.e. 64-bit x86 Macs.
Since Apple discontinued support for 32-bit applications on Mac OS X 10.15 (Catalina), Virgil runs only on the JVM on later versions.
You will work on the runtime and system layer of Virgil and make small modifications to the compiler to allow system calls and emit 64-bit MachO binaries.
You can base much of your work on the X86-32 runtime.
IMPACT: You will make it possible to develop Virgil and Wizard natively on MacOS X 10.15 and later.
Compiler and assembly experience required.

### [Port Virgil to ARM64](PortVirgilARM64.md) - Virgil, fair difficulty, low novelty

In this project, you will port Virgil to the ARM64 architecture by writing a new assembler and compiler backend.
You will work on the internals of the Virgil compiler and deal with copious amounts of assembly code, becoming an expert on compiler backends.
You can base much of your work on the X86-64 backend.
IMPACT: You will make it possible to develop Virgil and Wizard on the wonderful new M1 line of Macs.
Compiler and assembly experience required.

### [Port Wizard to ARM64](PortWizardARM64.md) - Wizard, moderate difficulty, moderate novelty

In this project, you will write a new interpreter (and potentially JIT backend) for Wizard in ARM64 assembly code.
You will need Virgil to first be ported to ARM64.
IMPACT: You will make it possible to develop Wizard on the wonderful new M1 line of Macs.
Assembly and WebAssembly experience required.

### [Port Virgil to RISC-V](PortVirgilRISCV.md) - Virgil, fair difficulty, low novelty

In this project, you will port Virgil to the RISC-V architecture by writing a new assembler and compiler backend.
You will work on the internals of the Virgil compiler and deal with copious amounts of assembly code, becoming an expert on compiler backends.
You can base much of your work on the X86-64 backend.
IMPACT: You will make Virgil run on an exciting new line of hardware.
Compiler and assembly experience required.
