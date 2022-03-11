# Student projects

In this repo, you will find an up-to-date list of projects of various sizes and difficulties for students interested in working with me on class, research, or honors projects.
Some projects have a larger component of research (i.e. high novelty, many unknowns) than others.

** [Packing ADTs](PackingADTs.md) ** - Virgil, moderate difficulty, high novelty

In this project, you will explore new techniques to represent algebraic data types (ADTs) more efficiently.
You will work on the internals of a sophisticated, static compiler for the Virgil programming language and introduce new analysis and optimizations in this compiler.
IMPACT: You will make Virgil completely outclass all languages to date and very likely publish a paper.
Compiler experience and some familiarity with functional programming required.

** [Data Layouts](DataLayouts.md) ** - Virgil, moderate difficulty, high novelty

In this project, you will design and implement new language constructs for describing memory layouts of fixed data structures such as network packets, kernel buffers, etc.
You will work on the internals of a sophisticated, static compiler for the Virgil programming language and introduce new analysis and optimizations in this compiler.
IMPACT: You will make Virgil the language of choice for low-level programming where memory layouts are fixed and likely publish a paper.
Compiler experience required.

** [Partial Specialization](PartialSpecialization.md) ** - Virgil, moderate difficulty, high novelty

In this project, you will explore new ways to implement polymorphic types.
You will work on the internals of a sophisticated, static compiler for the Virgil programming language and introduce new analysis and optimizations in this compiler.
You will investigate sharing polymorphic specializations before specialized code is generated.
IMPACT: You will make Virgil obliterate other languages with polymorphic types and very likely publish a paper.
Compiler experience and some programming language theory required.

** [Benchmark WebAssembly](BenchmarkWasm.md) ** - WebAssembly, fair difficulty, fair novelty

In this project, you will scour the planet for benchmarks for WebAssembly, creating a suite of freely-available kernels, micro-benchmarks, programs, and applications that is useful for studying all aspects of Wasm performance.
You will follow best practices from benchmarking literature and known suites such as SPEC and DaCapo and create a framework for easily obtaining statistically reliable, reproducible results.
IMPACT: You will make it easy to reliably benchmark any aspect of any Wasm engine and maybe publish the go-to paper on doing so.
Basic programming and scripting experience required, some familiarity with statistics.

** [MMTk for Virgil](MMTkVirgil.md) ** - Virgil, Rust, moderate difficulty, moderate novelty

In this project, you will aim to improve Virgil's garbage collection performance by interfacing with MMTk, a modern, high-performance, VM-agnostic GC framework.
You will work out how to interface the MMTk runtime with Virgil's runtime and develop necessary compiler modifications for the interoperability.
IMPACT: You will make Virgil GC state-of-the-art and maybe publish a paper.
Compiler experience and some familiarity with GC required.

** [Graph Coloring Register Allocator](RegAlloc.md) ** - Virgil, high difficulty, moderate novelty

In this project, you will write a new, sophisticated register allocator for the advanced Virgil compiler.
Despite being studied for five decades, register allocation remains a challenging problem.
You will explore new techniques to make graph coloring register allocation more efficient, in particular better
splitting heuristics and incremental rebuilding of the interference graph.
IMPACT: You will make Virgil run much faster and maybe publish a paper.
Compiler experience required.

** [Port Wizard's Fast Interpreter to JSC](PortWizardJSC.md) ** - C++, WebAssembly, high difficulty, moderate novelty

In this project, you will port (or rewrite) Wizard's fast in-place interpreter, hand-written in assembly, to JavaScriptCore.
You will add a new (or adapt the existing) interpreter tier which does not rewrite Wasm, but uses the original bytes.
IMPACT: You will demonstrate that WebAssembly can be interpreted in-place fast in a production engine and maybe publish a paper.
Assembly and C++ experience required.

** [Port Virgil to ARM64](PortVirgilARM64.md) ** - Virgil, fair difficulty, low novelty

In this project, you will port Virgil to the ARM64 architecture by writing a new assembler and compiler backend.
You will work on the internals of the Virgil compiler and deal with copious amounts of assembly code, becoming an expert on compiler backends.
You can base much of your work on the X86-64 backend.
IMPACT: You will make it possible to develop Virgil and Wizard on the wonderful new M1 line of Macs.
Compiler and assembly experience required.

** [Port Wizard to ARM64](PortWizardARM64.md) ** - Wizard, moderate difficulty, moderate novelty

In this project, you will write a new interpreter (and potentially JIT backend) for Wizard in ARM64 assembly code.
You will need Virgil to first be ported to ARM64.
IMPACT: You will make it possible to develop Wizard on the wonderful new M1 line of Macs.
Assembly and WebAssembly experience required.

** [Port Virgil to RISC-V](PortVirgilRISCV.md) ** - Virgil, fair difficulty, low novelty

In this project, you will port Virgil to the RISC-V architecture by writing a new assembler and compiler backend.
You will work on the internals of the Virgil compiler and deal with copious amounts of assembly code, becoming an expert on compiler backends.
You can base much of your work on the X86-64 backend.
IMPACT: You will make Virgil run on an exciting new line of hardware.
Compiler and assembly experience required.
