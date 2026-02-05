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

### [Partial Specialization](PartialSpecialization.md) - Virgil, moderate difficulty, high novelty

In this project, you will explore new ways to implement polymorphic types.
You will work on the internals of a sophisticated, static compiler for the Virgil programming language and introduce new analysis and optimizations in this compiler.
You will investigate sharing polymorphic specializations before specialized code is generated.
IMPACT: You will make Virgil obliterate other languages with polymorphic types and very likely publish a paper.
Compiler experience and some programming language theory required.

### [MMTk for Virgil](MMTkVirgil.md) - Virgil, Rust, moderate difficulty, moderate novelty

In this project, you will aim to improve Virgil's garbage collection performance by interfacing with MMTk, a modern, high-performance, VM-agnostic GC framework.
You will work out how to interface the MMTk runtime with Virgil's runtime and develop necessary compiler modifications for the interoperability.
IMPACT: You will make Virgil GC state-of-the-art and maybe publish a paper.
Compiler experience and some familiarity with GC required.

## Development Projects

Writing code in Virgil is a lot of fun, but tooling support can always be better.
Several projects could help make Virgil a lot more productive.

### Integrate with [Visual Studio Code](https://code.visualstudio.com/api/language-extensions/overview)

A popular, fast, and extensible editor, Visual Studio Code supports a range of integration levels for new languages.
In this project, you'll extend Visual Studio Code with syntax highlight, bracket matching, and eventually, completion.
Implement a language server that will allow checking syntax errors directly in the editor and improve the development experience for all Virgil programmers!

## Feature Projects

Both Virgil (the programming language) and Wizard (the WebAssembly engine) can benefit from new features.
Adding new features to the Virgil programming language not only makes writing code more fun and expressive, but can enable new types of expression patterns and accompanying compiler optimizations that make VM development a whole lot nicer.
In particular, the Wizard engine should stay up-to-date with coming proposals, but also support platform features (like WASI) that make it possible to experiment with large, real programs.

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

## In-progress projects

### [Implement `wasi_snapshot_preview1` in Wizard on `x86-64-linux`](WasiWizard.md) - Virgil, low difficulty, low novelty, high priority

In this project, you will implement the WebAssembly System Interface (WASI) in the Wizard Engine.
You'll write code to interface directly with the Linux kernel to provide the lowest-overhead, no-dependency implementation of this interface.
IMPACT: You will greatly improve the number of applications Wizard can run, allowing testing, benchmarking, and studying full applications in direct comparison to production engines.
WebAssembly experience required, low-level system call familiarity required.

## Completed (or mostly completed) projects

### [Port Wizard's Fast Interpreter to JSC](PortWizardJSC.md) - C++, WebAssembly, high difficulty, moderate novelty

This was already done by the JSC team and is now part of Safari.

### [Benchmark WebAssembly](BenchmarkWasm.md) - WebAssembly, fair difficulty, fair novelty

This project is mostly completed with [Wasure](https://github.com/r-carissimi/wasure).

### [Port Virgil to x86-64-darwin](PortVirgilX8664Darwin.md) - Virgil, low difficulty, low novelty, high priority

This project is complete.

### [Design a Data Layout Embedded DSL for Virgil](DataLayouts.md) - Virgil, moderate difficulty, high novelty

This project consists of two parts: [layouts](https://github.com/titzer/virgil/blob/master/doc/tutorial/Layouts.md) and [packing](https://dl.acm.org/doi/10.1145/3694848.3694857) and is mostly completed.

### [Graph Coloring Register Allocator](RegAlloc.md) - Virgil

This project is mostly completed, however coalescing is currently turned off, and a better splitting mechanism could be implemented.
Maintenance / refactoring now.

