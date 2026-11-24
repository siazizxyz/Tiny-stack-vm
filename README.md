# tiny-stack-vm

A tiny stack virtual machine for make.fun bounty `tiny-stack-vm-01-run-20261122`.

`main.ts` is a faithful interpreter of the ISA (`generator/subject/ISA.md` in
the kit): exact 32-bit wrapping arithmetic, unsigned DIV/MOD/LT, shifts masked
to 5 bits, and all ten traps with their own exit codes, plus the stack, call,
memory, step and output limits. Node 22 runs `node /bot/main.ts`; it reads
every instance from `$MAKEFUN_INPUT_DIR/<id>/{program,input}.bin` and writes
`$MAKEFUN_OUTPUT_DIR/<id>/{stdout.bin,exit.txt}`.

Practice set: 40/40 instances, score 1,000,000.
