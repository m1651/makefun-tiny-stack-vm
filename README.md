# tiny-stack-vm

A faithful interpreter of make.fun's tiny stack ISA (version 1) for the
"Build a tiny stack virtual machine, 22 November 2026" bounty: 32-bit
wrapping arithmetic, a 256-value stack, calls, 256 words of memory,
input/output, and all ten traps with their own exit codes, including
the hard rules (wrapping MUL, DIV/MOD edge cases, unsigned DIVU/MODU/
LTU, 5-bit shifts, SHR vs SHRU, PUSH8 sign extension, step/output
limits). One run answers all 40 instances of a set.

## Run it

```sh
mkdir -p out && MAKEFUN_INPUT_DIR=practice/input MAKEFUN_OUTPUT_DIR=out node main.ts
```

Owner/repo: m1651/makefun-tiny-stack-vm
Referral code: wwm9ek0a
