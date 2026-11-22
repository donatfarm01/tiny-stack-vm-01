# Tiny Stack VM

A faithful interpreter of make.fun's tiny stack ISA: runs every bytecode program in a set and writes its exact stdout bytes and exit code, traps included.

[![tiny-stack-vm-01-run-20261122](https://make.fun/badge/tiny-stack-vm-01-run-20261122.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122)
[![Rank](https://make.fun/badge/tiny-stack-vm-01-run-20261122/donatfarm01/tiny-stack-vm-01/rank.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122)
[![Reward](https://make.fun/badge/tiny-stack-vm-01-run-20261122/donatfarm01/tiny-stack-vm-01/reward.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122)

Run locally on the practice set (from the unpacked kit):

```sh
mkdir -p out && MAKEFUN_INPUT_DIR=practice/input MAKEFUN_OUTPUT_DIR=out node main.ts
```

Scores 1,000,000 on the practice set: every instance's stdout and exit code match the reference VM, beating the house baseline plain-vm 1.0.0 (670,000). See BUILD-NOTES.md.
