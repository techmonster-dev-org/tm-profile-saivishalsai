# Computer Architecture & Systems (How the Machine Really Works) — Full Track Record

**saivishalsai** · [← Back to profile](../README.md) · Updated 2026-10-24

## Progress

[░░░░░░░░░░░░░░░░░░░░] 0%   (0 of 48 projects completed)

## Data, Numbers & Representation

| Project | Score | Understanding | Reviewed | Feedback |
|---|---|---|---|---|
| Encode and decode signed and unsigned integers in binary using two's complement, observe sign extension, and query type ranges with std::numeric_limits. | ⬜ Not started | — | — | — |
| Explore unsigned wraparound vs signed undefined behavior, reproduce the unsigned-comparison trap and size-calculation vulnerability, and implement safe overflow-detecting arithmetic. | ⬜ Not started | — | — | — |
| Design, write, and read a fixed 16-byte binary record format with magic number, little-endian integer fields, and an XOR checksum using std::fstream in binary mode, synthesizing all Phase 1 concepts. | ⬜ Not started | — | — | — |
| Expose the integer nature of char, print the ASCII table, manually decode UTF-8 byte sequences to Unicode code points, and implement a code-point iterator that correctly handles multi-byte characters. | ⬜ Not started | — | — | — |
| Apply all six bitwise operators to implement bitmask flag operations, model a hardware register with C++ bit-fields, and measure struct padding and alignment with sizeof and offsetof. | ⬜ Not started | — | — | — |
| Decode the sign/exponent/mantissa bit layout of IEEE-754 floats, reproduce the 0.1+0.2 precision problem, inspect special values, and implement correct epsilon-based comparisons. | ⬜ Not started | — | — | — |
| Inspect multi-byte integer layout in memory, convert between host and network byte order using htonl/ntohl, type-pun safely with std::memcpy, and implement portable little/big-endian serialization. | ⬜ Not started | — | — | — |
| Inspect the raw binary and hex representation of C++ fundamental types using sizeof, std::bitset, fixed-width cstdint types, and byte-level memory access. | ⬜ Not started | — | — | — |

## From C to the Machine: Assembly & Linking

| Project | Score | Understanding | Reviewed | Feedback |
|---|---|---|---|---|
| Compile a complete C++ program, disassemble it with objdump -d -M intel, and produce a fully annotated walkthrough of dot_product and argmax — mapping every instruction back to the C++ source. | ⬜ Not started | — | — | — |
| Decode the x86-64 base+index*scale+displacement addressing formula by tracing how array indexing, struct field access, and pointer arithmetic each compile to a specific memory operand. | ⬜ Not started | — | — | — |
| Compare -O0 and -O2 compiler output for local variables, arithmetic, dead code, and constant folding — making the compiler's translation rules and optimization license visible. | ⬜ Not started | — | — | — |
| Walk a two-file C++ program through all four pipeline stages — preprocess, compile, assemble, link — stopping at each to read the intermediate file and inspect symbols with nm. | ⬜ Not started | — | — | — |
| Learn the x86-64 register file, Intel syntax, and the core instruction set by annotating compiler output on Compiler Explorer — turning assembly from noise into readable machine-level C++. | ⬜ Not started | — | — | — |
| Trace the System V AMD64 ABI from argument registers through stack frame layout, prologue/epilogue, call/ret mechanics, and the red zone — building a complete mental model of how every function call works at the hardware level. | ⬜ Not started | — | — | — |
| Trace how if/else, for/while loops, and switch statements compile to cmp, conditional jumps, loop labels, and jump tables — making the FLAGS register and branchy assembly readable. | ⬜ Not started | — | — | — |
| Build a static and a dynamic library, inspect symbols with nm/objdump/readelf, trigger a linker error to understand ODR, and learn the difference between static (.a) and dynamic (.so) linking. | ⬜ Not started | — | — | — |

## The Processor & Performance

| Project | Score | Understanding | Reviewed | Feedback |
|---|---|---|---|---|
| Reproduce the classic sorted-vs-unsorted array benchmark, quantify the ~15-cycle misprediction penalty, and implement branchless alternatives using arithmetic masking and cmov. | ⬜ Not started | — | — | — |
| Break single-accumulator dependency chains with multiple accumulators, measure the IPC improvement via perf stat, and apply the pattern to both integer and FP reduction loops. | ⬜ Not started | — | — | — |
| Take a naive character-frequency histogram from 0.35 GB/s to 7.8 GB/s by applying four bottleneck-targeted optimizations in sequence, profiling with perf at each step, and producing a full optimization report. | ⬜ Not started | — | — | — |
| Measure the performance impact of -O0 through -Ofast, observe constant folding and inlining with timing experiments, use __restrict__ to unblock auto-vectorization, and read generated assembly on Compiler Explorer. | ⬜ Not started | — | — | — |
| Build a three-bottleneck target program, profile it with perf stat and perf record, identify each hotspot by its counter signature, and generate a flamegraph to visualize the call stack. | ⬜ Not started | — | — | — |
| Apply four targeted optimizations to a deliberately slow order-processing function — eliminating heap allocations, hoisting invariants, replacing branches with lookup tables, and transforming AoS to SoA — and document a measurement log for each step. | ⬜ Not started | — | — | — |
| Build a series of C++ microbenchmarks that make pipeline throughput, latency, data hazards, and superscalar IPC visible and measurable. | ⬜ Not started | — | — | — |
| Measure your machine's peak memory bandwidth and peak FLOPs, calculate arithmetic intensity for three kernels, place them on a roofline diagram, and determine which optimizations help in each performance regime. | ⬜ Not started | — | — | — |

## The Memory Hierarchy & Caches

| Project | Score | Understanding | Reviewed | Feedback |
|---|---|---|---|---|
| Build a pointer-chasing benchmark that measures access latency across L1/L2/L3/DRAM and internalise the canonical latency numbers that drive every systems-performance decision. | ⬜ Not started | — | — | — |
| Build a stride benchmark that exposes cache-set conflicts by exploiting tag/index/offset address geometry, and measure L1/L2/L3/DRAM hit latency directly. | ⬜ Not started | — | — | — |
| Implement a cache-line-sized B-tree node (15 int32 keys per 64-byte node), benchmark it against sorted-array binary search and a linked list, and explain the full speedup using every principle from Phase 4. | ⬜ Not started | — | — | — |
| Build a 2D throughput table sweeping working-set size and stride to map L1/L2/L3/DRAM plateaus and identify the spatial- and temporal-locality ridges on the student's own machine. | ⬜ Not started | — | — | — |
| Measure the TLB miss cliff by striding through a 256 MB array in page-sized increments, identify TLB capacity on the student's machine, and explain paging, page faults, and huge pages. | ⬜ Not started | — | — | — |
| Benchmark AoS vs SoA particle layouts for a field-selective loop, measure the cache-utilisation speedup, and learn when each layout is correct using data-oriented design principles. | ⬜ Not started | — | — | — |
| Measure the row-major vs column-major 2D traversal gap and fix a matrix-multiply loop order, explaining every speedup in cache-line terms. | ⬜ Not started | — | — | — |
| Reproduce and measure a false-sharing slowdown with two threads, fix it with alignas(64) padding and per-thread local accumulation, and explain the MESI coherence mechanism behind the bug. | ⬜ Not started | — | — | — |

## Concurrency at the Hardware Level

| Project | Score | Understanding | Reviewed | Feedback |
|---|---|---|---|---|
| Build the broken and correct flag-plus-data handoff, benchmark seq_cst vs acquire/release vs relaxed, and explain operationally what each ordering permits the CPU and compiler to reorder. | ⬜ Not started | — | — | — |
| Parallelize a histogram workload across N threads, measure speedup vs cores, diagnose false sharing and load imbalance, and fit Amdahl's Law to predict the serial-fraction ceiling. | ⬜ Not started | — | — | — |
| Query hardware topology, measure context-switch cost, demonstrate oversubscription collapse, and pin threads to specific CPU cores using pthread_setaffinity_np. | ⬜ Not started | — | — | — |
| Build a correct atomic counter three ways, implement a CAS retry loop, construct a spinlock from std::atomic_flag, and benchmark atomic vs mutex performance. | ⬜ Not started | — | — | — |
| Vectorize a float-array kernel using AVX2 intrinsics and auto-vectorization, measure scalar vs SIMD throughput, and understand alignment requirements and horizontal reduction. | ⬜ Not started | — | — | — |
| Build a correct single-producer/single-consumer ring buffer using acquire/release atomics, demonstrate cache-line separation of head and tail, and benchmark against a mutex queue. | ⬜ Not started | — | — | — |
| Measure single-mutex throughput collapse vs thread count, recover scaling with per-bucket fine-grained locks, and quantify cache-line bounce and spinlock vs blocking-mutex trade-offs. | ⬜ Not started | — | — | — |
| Observe compiler and hardware reordering, detect data races with ThreadSanitizer, and build the happens-before mental model that makes concurrent code provably correct. | ⬜ Not started | — | — | — |

## The OS Interface & Low-Latency Systems

| Project | Score | Understanding | Reviewed | Feedback |
|---|---|---|---|---|
| Build, measure, and package a lock-free SPSC ring buffer with std::atomic acquire/release ordering and alignas(64) cache-line isolation, instrument it with a latency histogram reporting p50/p99/p99.9, benchmark it head-to-head against a mutex baseline and a naive (false-sharing) variant, and package everything with CMake + GoogleTest — the portfolio artifact that closes the Computer Architecture & Systems track. | ⬜ Not started | — | — | — |
| Use the POSIX open/read/write/close/mmap syscall family to read a 1 MiB file at multiple chunk sizes, measure the throughput gap between per-byte and batched reads, and then memory-map the same file to observe zero-copy access — connecting each strategy to the kernel page cache. | ⬜ Not started | — | — | — |
| Build a TCP echo server and client from raw POSIX syscalls (socket/bind/listen/accept/connect/send/recv), handle partial sends and receives correctly, measure loopback round-trip latency, and learn the socket options that matter for low-latency systems. | ⬜ Not started | — | — | — |
| Build a single-threaded TCP echo server using epoll_create/epoll_ctl/epoll_wait that handles multiple simultaneous non-blocking clients, implement edge-triggered drain loops, and explain why the reactor pattern scales to 10,000 connections where blocking-per-connection does not. | ⬜ Not started | — | — | — |
| Install signal handlers with sigaction(2) to implement graceful SIGINT/SIGTERM shutdown, demonstrate why printf is banned in signal handlers, observe EINTR from interrupted syscalls, and implement the self-pipe trick to integrate signals safely into a select-based event loop. | ⬜ Not started | — | — | — |
| Use fork(2) to create child processes and observe copy-on-write address-space isolation, communicate between processes with a pipe, benchmark process vs thread creation cost, and explain when each abstraction is the right tool for a latency-critical system. | ⬜ Not started | — | — | — |
| Measure the cost of a mode switch by writing programs that call write(2) directly, watching every syscall with strace, and benchmarking batched vs. per-byte writes — then explain why HFT hot paths obsess over eliminating kernel crossings. | ⬜ Not started | — | — | — |
| Synthesize the HFT engineering toolkit: implement and benchmark busy-polling vs epoll wakeup latency, apply the no-alloc hot-path discipline and measure p99 improvement, pin threads to CPU cores, and explain kernel-bypass concepts (DPDK, a kernel-bypass NIC) — backed by a latency histogram reporting p50/p99/p99.9. | ⬜ Not started | — | — | — |

---
*Machine-readable proof with commit SHA anchors: [verified-record.json](./verified-record.json)*