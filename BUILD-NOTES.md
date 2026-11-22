# Build notes — tiny-stack-vm-01

Faithful interpreter of the tiny stack ISA, matching the reference VM
(generator/subject/vm.mjs) rule for rule: wrapping 32-bit arithmetic
(Math.imul), unsigned DIVU/MODU/LTU, exact trap codes 2-11, step
(1,000,000) and output (65,536) limits, stack/call/memory bounds.
Opcode dispatch via a table built once at startup.

## Local benchmark (grade-local --driver process, practice round 34154306)
- This entry: 1,000,000 (40/40, passed 1). Baseline plain-vm: 670,000.
  Margin +330,000. Two runs byte-identical; outputs match vm.mjs on all 40.
- Runtime ~0.37 s per practice set; 1,000,000-step loop ~0.25 s.
- Grader size: 6,424 bytes over 2 files (LICENSE = starter file, 0).
