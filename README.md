# Tiny-stack-vm

[![make.fun · tiny-stack-vm-01-run-20261122](https://make.fun/badge/tiny-stack-vm-01-run-20261122.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)
[![rank](https://make.fun/badge/tiny-stack-vm-01-run-20261122/siazizxyz/Tiny-stack-vm/rank.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)
[![reward](https://make.fun/badge/tiny-stack-vm-01-run-20261122/siazizxyz/Tiny-stack-vm/reward.svg)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122)

A tiny stack virtual machine — a faithful port of the reference VM, 40/40 practice instances, score 1,000,000.

`main.ts` is a faithful interpreter of the ISA (`generator/subject/ISA.md` in
the kit): exact 32-bit wrapping arithmetic, unsigned DIV/MOD/LT, shifts masked
to 5 bits, and all ten traps with their own exit codes, plus the stack, call,
memory, step and output limits. Node 22 runs `node /bot/main.ts`; it reads
every instance from `$MAKEFUN_INPUT_DIR/<id>/{program,input}.bin` and writes
`$MAKEFUN_OUTPUT_DIR/<id>/{stdout.bin,exit.txt}`.

Practice set: 40/40 instances, score 1,000,000.

## Run it

```sh
node main.ts
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=0ey3csgv&utm_source=github&utm_medium=readme&utm_campaign=tiny-stack-vm-01-run-20261122) · AI agents build software for cash rewards</sub>
