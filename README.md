# Letter of Recommendations for Bao

For Professor Ratan Dey.

## Schools List and Deadlines

| **School** | **Letter Deadline** | **Status** |
| --- | --- | --- |
| University of California, Berkeley | January 5, 2027 | Not Requested by Program Yet |
| Columbia University | January 14, 2027 | Not Requested by Program Yet |
| Northwestern University | January 14, 2027 | Not Requested by Program Yet |
| University of Michigan | January 14, 2027 | Not Requested by Program Yet |
| Carnegie Mellon University | January 14, 2027 | Not Requested by Program Yet |
| Cornell University | January 14, 2027 | Not Requested by Program Yet |
| University of Pennsylvania | January 14, 2027 | Not Requested by Program Yet |

## What I Am Applying For and Why

I am applying to master's programs to build on my electrical engineering preparation, including the microarchitecture work I did in your course and Processor Design. I want to understand how microcontrollers in embedded devices use processing and memory resources to acquire and analyze data. Further study in this area, alongside control theory and digital signal processing, would support my goal of starting my own company that develops neural recording and analysis tools.

## Academic Performance

### My Courses with You

- Computer Architecture (CS-UY 2214): A-

### General

- Overall GPA: 3.677/4.000
- Advanced GPA (final 2 years): 3.896/4.000

## Resume

[View my resume (PDF)](Bao-Nguyen_resume.pdf)

## How You Know Me

### My Courses With You

- Computer Architecture (CS-UY 2214): A-

### Projects

- Team member of your VIP team Processor Design.

## Specific Work You Have Seen Me Do

### Processor Design VIP

| **Timeline** | **My Contribution** | **Outcomes** |
| --- | --- | --- |
| March 2026 | **RiSC-16 Onboarding Project:**<br>Co-developed the instruction and data memories, program counter, register file, ALU, and processor integration with Tim. | • Compiled and ran the integrated processor with the supplied testbench, obtaining the expected outputs.<br>• Connected separately developed components into a processor that could be exercised together. |
| March 2026 | **Onboarding Labs:**<br>Implemented SystemVerilog exercises and configured the CMake/C++ onboarding workflow. | • Applied combinational and sequential logic through an ALU, LFSR, module composition, and decoder/mux.<br>• Gained practice configuring CMake and organizing C++ sources within the onboarding build workflow. |
| May 2026 | **Configurable Instruction Decoder Proposal:**<br>Co-presented a SKY130 decoder architecture and its planned verification, synthesis, physical-design, and signoff process. | • Made the relationships between decoder architecture, verification, synthesis, physical design, and signoff explicit.<br>• Presented implementation milestones and tradeoffs for team discussion; the design remained a proposal. |
| September 2026 | **Onboarding Lab Support:**<br>Assisted Hans and Paul with assessments and recommended corrections to test completion, watchdogs, SystemVerilog explanations, and parameter constraints. | • Provided leads with concrete feedback on combinational behavior, simulation startup, and single-writer restrictions.<br>• Recommended passing criteria and separate watchdogs so successful checks and stalled tests would be distinguishable. |
| September 2026 | **JAL Datapath and Control Design:**<br>Mapped immediate generation, jump-target calculation, return-address writeback, and connections to shared adders and multiplexers. | • Made jump-target calculation and return-address writeback explicit within the shared datapath.<br>• Identified interface connections and control requirements, while leaving mux encodings and exception handling for shared integration decisions. |
| October 2026 | **RV32I Top-Level Processor Integration:**<br>Connected six core modules, added guarded instruction memory, built the top-level smoke testbench, and strengthened lint and runner checks. | • Recorded Level 1 checks reported 3 passes, 0 failures, and 4 skips.<br>• The smoke test confirmed clocked simulation completion; functional verification remained pending because dependencies were unfinished. |

### Microcontroller

[Project repository](https://github.com/baolgn/microcontroller)

| **Timeline** | **My Contribution** | **Outcomes** |
| --- | --- | --- |
| October 2026 | **Architecture and Development Plan:**<br>Defined the instruction-set and machine-state contract, timing budgets, FPGA target, and development tools before RTL implementation. | • Established an explicit instruction-set and machine-state contract before RTL implementation.<br>• Defined timing assumptions and verification boundaries so later results could be assessed against stated requirements. |
| November 2026 | **Five-Stage Pipeline and Instruction Execution:**<br>Implemented decoding, arithmetic, control flow, dependency forwarding, load-use stalls, tagged fetches, and ordered retirement. | • Recorded 1,020 cycles with forwarding versus 2,131 in diagnostic mode across the same 53-case simulated workload.<br>• Execution traces made pipeline overlap and dependency handling directly observable. |
| November 2026 | **Memory, Exceptions, and Interrupts:**<br>Implemented aligned memory accesses, precise traps, machine CSRs, retained interrupts, and WFI wakeup while preserving request ownership. | • Retained outstanding requests through stalls and hart resets in the tested scenarios.<br>• Separate memory-effect checks can expose duplicate or unowned accesses even when final register values appear correct. |
| November 2026 | **Instruction Extensions and Synchronization:**<br>Added multiplication/division, compressed instructions, memory fences, instruction synchronization, machine counters, and tests for arithmetic and execution corner cases. | • Checked all 65,536 halfword encodings across legal, illegal, HINT, and wide-prefix classifications.<br>• Multiplication and division produced valid results 2 and 33 clocks after acceptance, respectively. |
| November 2026 | **Local Platform and Firmware:**<br>Integrated local memories, timers, and MMIO with C/assembly firmware, including startup, trap handling, and exception recovery. | • Passed 12 positive firmware simulations and 3 injected-fault detector tests.<br>• Startup and trap handling supported compiled C/assembly execution without hiding initialization defects through preloaded data memory. |
| November 2026 | **FPGA Tools and Boot Recovery:**<br>Implemented synthesis/routing tooling, firmware image validation, dual-bank updates, and simulated recovery from damaged or empty firmware banks. | • Passed 9 simulations covering normal boot and damaged-bank recovery.<br>• Preserved the golden firmware bank during normal updates; physical flash behavior and power-cycle recovery remain unverified. |
| November 2026 | **Debug Control and Simulator Integration:**<br>Implemented halt, resume, single-step, register access, JTAG transport, and simulated OpenOCD/GDB integration. | • Simulated halt and single-step enabled register inspection at defined execution and fault boundaries.<br>• Tests detected injected faults in reset retention and code write protection; physical debug probe operation remains unverified. |
| November 2026 | **Processor Verification and Reference Comparison:**<br>Built directed tests, randomized execution checks, Sail comparisons, and bounded formal harnesses, checking retirement and memory effects separately. | • Combined independent instruction-result and memory-effect checks with directed, randomized, reference-model, and bounded formal verification.<br>• Architectural comparison gaps remain open; these checks do not establish complete processor correctness. |
| November 2026 | **Reproducible Testing and Waveform Analysis:**<br>Created waveform explanations with provenance records and automated isolated acceptance, dependency checks, and release-archive validation. | • Checked waveform captions against passing simulations, making hazards, traps, and memory ownership inspectable at specific clock edges.<br>• Source and tool records support tracing and repeating observations. |

### Coursework

| **Timeline** | **My Contribution** | **Outcomes** |
| --- | --- | --- |
| October 2025 | **E20 Processor Simulator (CS-UY 2214):**<br>Implemented machine-code execution, processor-state updates, and final-state reporting. | • Produced a simulator for an eight-register processor with 8,192 memory cells.<br>• Made instruction-driven state changes observable through a final report of registers, memory, and the program counter. |
| November 2025 | **E20 Cache Simulator (CS-UY 2214):**<br>Implemented configurable L1/L2 caches, LRU replacement, write-through/write-allocate behavior, event logging, and custom assembly tests. | • Created 29 custom assembly tests with matching machine-code files for cache behavior and corner cases.<br>• Made cache hits, misses, and writes observable across configurable cache hierarchies. |
| December 2025 | **Course Completion (CS-UY 2214):**<br>Studied digital logic, processor datapaths, pipelining, caches, virtual memory, and assembly programming. | • Learned how datapath and control choices govern instruction execution, and how pipeline hazards affect performance.<br>• Connected caching and virtual memory to memory-system behavior; earned A- in CS-UY 2214. |

## 2 Qualities I Hope You Will Highlight

### Architectural Integration

- In Processor Design VIP, I mapped JAL's jump target and return address through shared adders and multiplexers, identifying immediate generation, bus widths, control signals, and remaining integration decisions.
  - This made the connections needed for jump-target calculation and return-address writeback explicit for team review, while keeping unresolved mux encodings and exception handling available for shared decisions.
- I applied systems thinking when integrating six core modules in `top.sv`, connecting operand selection, branch and jump paths, memory operations, and writeback while reconciling the byte-addressed PC with halfword instruction storage.
  - The team [approved and merged the top module and Level 1 testbench](https://github.com/NYU-Processor-Design/processor_design_vip_f26/pull/30), providing an accepted integration baseline for continuing processor development. The accompanying smoke test was limited to checking clocked simulation completion.
  - A team lead [built on this merged implementation](https://github.com/NYU-Processor-Design/processor_design_vip_f26/commit/6b18d071c1a5b7c298a6184d7316420263c3097a) by adding separate instruction memory and peripheral-bus connections.

### Technical Guidance

- After asking to assist the Processor Design VIP leads, I helped Hans and Paul assess the first onboarding lab for incoming members.
  - My assessment work provided additional review support for the leads during onboarding.
- I recommended clearer `always_comb` explanations, numeric arguments in failure calls, explicit passing criteria, separate watchdog timeouts, consistent signal widths, and valid parameter constraints for subsequent onboarding labs.
  - These recommendations supplied concrete guidance for distinguishing successful test completion, stalled tests, and invalid configurations, while clarifying the SystemVerilog behavior new members were learning.
- I strengthened the shared Level 1 test runner to reject failed commands, timeouts, and memory-image errors even when a test printed a success marker.
  - These failure conditions became explicit reasons to reject a run across the team's Level 1 tests, so a printed success message could not conceal them.
