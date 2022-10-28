- [repos](#repos)
- [papers](#papers)
- [books](#books)
- [blags](#blags)

# repos

## [Parameterizing Branch-and-Bound Search Trees to Learn Branching Policies](https://github.com/ds4dm/branch-search-trees)

## [angr is a platform-agnostic binary analysis framework](https://github.com/angr/angr)

angr's power comes not from it being an emulator, but from being able to execute with what we call symbolic variables. 

## [Apple AMX Instruction Set](https://github.com/corsix/amx)

potential target for low latency (or sparse?) stuff

## [SDSL - Succinct Data Structure Library](https://github.com/simongog/sdsl-lite)

gonna need this sooner or later 

## [GILP (Geometric Interpretation of Linear Programs)](https://github.com/engri-1101/gilp)

just useful for learning about BB (what about interior point?)

## [Symbolic Fourier-Motzkin elimination](https://github.com/stephane-caron/pyfme)

is this the actual basis of PIP?

## [Page-Visibility-User-Script](https://github.com/IceWreck/Page-Visibility-User-Script)

for hackerrank interviews...

## [islpy](https://github.com/inducer/islpy)

## [Solve puzzles. Learn CUDA.](https://github.com/srush/GPU-Puzzles)

## [Clockwork: Polyhedral Analysis for Hardware Accelerators](https://github.com/dillonhuff/clockwork)

## [AST-transformations (jetbrains)](https://github.com/JetBrains-Research/ast-transformations)

can i use this for a better python ast? also [https://plugins.jetbrains.com/docs/intellij/psi.html](https://plugins.jetbrains.com/docs/intellij/psi.html)

## [Entropy-Directed Scheduling ](https://github.com/chhzh123/Entropy-directed-scheduling)

implement for CIRCT?

## [Circle](https://github.com/rsta2/circle)

Circle is a C++ bare metal programming environment for the Raspberry Pi.

## [Easy creation of custom import hooks to experiment on alternatives to Python's syntax](https://github.com/aroberge/ideas)

basically does rewrite on import which enables python files to host alternative syntax. kind of cute but not really what i want

## [Optimization Modulo Theories examples](https://github.com/PatrickTrentin88/omt_python_examples)

static memory allocation problem can be formulated as LRA opt + XOR? also [https://optimathsat.disi.unitn.it/](https://optimathsat.disi.unitn.it/).

## [Symbolic Fourier-Motzkin elimination](https://github.com/stephane-caron/pyfme)

not sure

## [clan](https://github.com/periscop/clan)

Chunky Loop Analyzer: A Polyhedral Representation Extraction Tool for High Level Programs

compiling is annoying [af](https://gist.github.com/9a58e1aa96b83028da4462a08ce3f441)

- [ ] python bindings
- [ ] use clan to analyze python for loops

## [langcc](https://github.com/jzimmerman/langcc)

A Next-Generation Compiler Compiler

- [ ] use it to parse python into MLIR (using [mll](https://github.com/makslevental/mll))

## [The Yices SMT Solver](https://github.com/SRI-CSL/yices2)

- [ ] extract the BDD and combine with PIP

## [Intel Extension for MLIR](https://github.com/intel/mlir-extensions)

- [ ] use the python frontend to lower to affine

## [SymEngine](https://github.com/symengine/symengine)

if i'm gonna solve things symbolically (ie DSA) this might be useful

## [xeus-cling](https://github.com/jupyter-xeus/xeus-cling)

just take for a test drive

## [Binary Decision Diagrams](https://pyeda.readthedocs.io/en/latest/bdd.html)

use in combination with yices?

## [Parma Polyhedra Library (PPL)](https://github.com/jfmc/ppl)

how is it different from ISL? [sage bindings?](https://doc.sagemath.org/html/en/reference/numerical/sage/numerical/backends/ppl_backend.html). also [python bindings](https://github.com/haudren/pyparma)

## [TAMUparametric PPOPT](https://github.com/TAMUparametric/PPOPT)

can this solve DSA?

## [VPL (Verified Polyhedra Library)](https://github.com/VERIMAG-Polyhedra/VPL)

somewhere in here there's an implementation of a PIP solver

>Polyhedral projection is a main operation of the polyhedron abstract
domain. It can be computed via parametric linear programming (PLP),
which is more efficient than the classic Fourier-Motzkin elimination method.

^ hmm is that really true? i thought one relied on the other?

related to [this paper](https://core.ac.uk/download/pdf/265345708.pdf) (An efficient parametric linear programming solver and application to polyhedral projection)

## [CuPPy](https://github.com/tkralphs/CuPPy)

> A naive implementation of the Gomory cutting plane algorithm

is this faster than solving the CSP?

## [The Dynamic Runtime Inlining (DRTI) project](https://github.com/drti)

> The basic concept is to get the normal compiler front end like clang to emit its LLVM Intermediate Representation (IR) as a bitcode file, then run a custom LLVM pass over this to inject DRTI code at the appropriate places.

# papers

## [SCIL - Symbolic Constraints in Integer Linear programming](https://link.springer.com/content/pdf/10.1007/3-540-45749-6_11.pdf)

also https://software.cs.uni-koeln.de/scil/documentation/html/main.html

## [Bounded Search and Symbolic Inference for Constraint Optimization](https://www.ijcai.org/Proceedings/05/Papers/1571.pdf)

We present a novel algorithm for finite domain constraint optimization that generalizes branch-and-bound search by reasoning about sets of assignments rather than individual assignments.

## [High Throughput Low Latency Online Image Processing by GPU/FPGA Coprocessors Using RDMA Techniques](https://sc20.supercomputing.org/proceedings/doctoral_showcase/doc_showcase_pages/drs107.html)

the next step of the low latency work

## [A Lightweight Symbolic Virtual Machine for Solver-Aided Host Languages](https://homes.cs.washington.edu/~emina/doc/rosette.pldi14.pdf)

don't quite understand this but symbolic virtual machine is what i need for various parts of the static memory planning thing

## [Symbolic Optimization with SMT Solvers](https://pages.cs.wisc.edu/~aws/papers/popl14.pdf)

## [An Efficient Parametric Linear Programming Solver and Application to Polyhedral Projection](https://core.ac.uk/download/pdf/265345708.pdf)

## [Geometric Algorithm for Multiparametric Linear Programming](http://cse.lab.imtlucca.it/~bemporad/publications/papers/jota-mplp.pdf)

faster way to solve PIPs?

## [Reinforcement Learning for Integer Programming: Learning to Cut](http://proceedings.mlr.press/v119/tang20a/tang20a.pdf)

approx method for solving ILPs (learning). probably not that easy to implement (gym env?)

## [Efficiently Solving Repeated Integer Linear Programming Problems by Learning Solutions of Similar Linear Programming Problems using Boosting Trees](https://dspace.mit.edu/bitstream/handle/1721.1/93099/MIT-CSAIL-TR-2015-001.pdf?sequence=2&isAllowed=y)

approx method for solving ILPs (learning). probably easy to prototype using xgboost

## [Presburger Formulas and Polyhedral Compilation](https://libisl.sourceforge.io/tutorial.pdf)

isl official tutorial (read after completing pollylabs tuts)

## [Discovering faster matrix multiplication algorithms with reinforcement learning](https://www.nature.com/articles/s41586-022-05172-4)

>Interestingly, AlphaTensor finds algorithms with a larger number of additions compared with Strassen-square (or equivalently, denser decompositions), but the discovered algorithms generate individual operations that can be efficiently fused by the specific XLA33 grouping procedure and thus are more tailored towards the compiler stack we use.

## [A Scalable Approach to Exact Resource-Constrained Scheduling Based on a Joint SDC and SAT Formulation](https://www.csl.cornell.edu/~zhiruz/pdfs/sds-fpga2018.pdf)

implement in CIRCT

maybe this can be done using [or-tools](https://github.com/google/or-tools/issues/2014)?

maybe this can be done with [https://github.com/siala/Hybrid-Mistral](https://github.com/siala/Hybrid-Mistral)

## [Formulating Integer Linear Programs: A Rogues’ Gallery](http://faculty.nps.edu/dell/docs/Formulettes060425.pdf)

just good to know

## [Symbolic Optimization with SMT Solvers](https://pages.cs.wisc.edu/~aws/papers/popl14.pdf)

can this solve the DSA problem?

## [Lock-Free Data Structures](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.98.3363&rep=rep1&type=pdf)

just good to know

## [Clockwork: Resource-Efficient Static Scheduling for Multi-Rate Image Processing Applications on FPGAs](https://ieeexplore.ieee.org/document/9444097)

implement in CIRCT

## [Macro-embedding Compiler Intermediate Languages in Racket](https://www.williamjbowman.com/resources/wjb2022-hashlang-x64.pdf)

read after learning racket

# books

## [CMSC 430:  Design and Implementation of Programming Languages](https://www.cs.umd.edu/class/fall2022/cmsc430/Notes.html)

racket class on implementing small languages

## [PURELY FUNCTIONAL DATA STRUCTURES](https://doc.lagout.org/programmation/Functional%20Programming/Chris_Okasaki-Purely_Functional_Data_Structures-Cambridge_University_Press%281998%29.pdf)

probably useful for lockfree?

## [Game Programming Patterns](https://gameprogrammingpatterns.com/)

just good to know

## [Optimizing Compilers for Modern Architectures](https://www.elsevier.com/books/optimizing-compilers-for-modern-architectures/allen/978-0-08-051324-9)

required reading but i'll probably never get to it?

## [Types and Programming Languages](https://www.cis.upenn.edu/~bcpierce/tapl/)

required reading but i'll probably never get to it?

# blags/websites

## [An Introduction to Binary Decision Diagrams](https://news.ycombinator.com/item?id=32993015)

## [Building a Tiny Mutex](https://zig.news/kprotty/building-a-tiny-mutex-537k)

definitely need to know this for HFT

## [Race Conditions Can Be Useful for Parallelism](https://news.ycombinator.com/item?id=33054378)

## [The Solid-State Register Allocator](https://www.mattkeeter.com/blog/2022-10-04-ssra/)

suitable allocation algo for nns?

## [Static, Shared Dynamic and Loadable Linux Libraries](http://www.yolinux.com/TUTORIALS/LibraryArchives-StaticAndDynamic.html)

re the MLIR pass plugin project. also [https://developer.ibm.com/tutorials/l-dynamic-libraries/](https://developer.ibm.com/tutorials/l-dynamic-libraries/)

## [Practical Guide to Bare Metal C++](https://arobenko.github.io/bare_metal_cpp/)

maybe for bare metal arm but also maybe bare metal gpu

## [Boosting Inline Packet Processing Using DPDK and GPUdev with GPUs](https://developer.nvidia.com/blog/optimizing-inline-packet-processing-using-dpdk-and-gpudev-with-gpus/)

this is the next stage of the low latency project

also [https://forums.developer.nvidia.com/t/boosting-inline-packet-processing-using-dpdk-and-gpudev-with-gpus/212943)](https://forums.developer.nvidia.com/t/boosting-inline-packet-processing-using-dpdk-and-gpudev-with-gpus/212943))
and [Benchmarking GPUDirect RDMA on Modern Server Platforms](https://developer.nvidia.com/blog/benchmarking-gpudirect-rdma-on-modern-server-platforms/)

## [mp-LE, explicit solutions](https://dkenefake.github.io/blog/mpLE)

can this solve the DSA problem?

## [Blossom algorithm](https://en.wikipedia.org/wiki/Blossom_algorithm)

should probably know this after teaching rohan

## [Procedural Macros: Parsing custom syntax](https://blog.turbo.fish/proc-macro-parsing/)

learn in order to use rust a compiler. another [source](https://developerlife.com/2022/03/30/rust-proc-macro/#eg-2---function-like-macro-that-parses-custom-syntax).

## [VLIW, Software Pipelining, and Limits to ILP](https://people.eecs.berkeley.edu/~pattrsn/252F96/Lecture05.pdf)

read in prep for luminous

## [hn post about autodiff in haskell](https://news.ycombinator.com/item?id=32879734)

some useful discussion on symbolic autodiff

## [hn post about Measuring CPU core-to-core latency](https://news.ycombinator.com/item?id=32889337)

useful for ... everything?

## [A look at the performance of expression templates in C++: Eigen vs Blaze vs Fastor vs Armadillo vs XTensor](https://romanpoya.medium.com/a-look-at-the-performance-of-expression-templates-in-c-eigen-vs-blaze-vs-fastor-vs-armadillo-vs-2474ed38d982)

probably inflated but worth a read

## [hn post about compiling Clang to WASM](https://news.ycombinator.com/item?id=30991235)

compile MLIR to wasm in order to run in browser? maybe that's useless and just use torch-mlir wheels

## [PCIe latency](http://hackingnasdaq.blogspot.com/2014/05/pcie-latency.html?m=1)

hack pcie to get lower than 0.5us latency

## [Simplification of Presburger formulas in practice](https://cstheory.stackexchange.com/questions/21281/simplification-of-presburger-formulas-in-practice)

cs.theory discussing how presburger formulas actually work - including some discussion of BDDs
