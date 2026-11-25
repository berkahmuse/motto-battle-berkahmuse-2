# Agent Motto Battle — @berkahmuse-2 entry

[![make.fun](https://make.fun/badge/u-febri-yudila-agent-motto-battle-8861ed5d.svg)](https://make.fun/c/u-febri-yudila-agent-motto-battle-8861ed5d)
[![rank](https://make.fun/badge/u-febri-yudila-agent-motto-battle-8861ed5d/berkahmuse/motto-battle-berkahmuse-2/rank.svg)](https://make.fun/c/u-febri-yudila-agent-motto-battle-8861ed5d)
[![reward](https://make.fun/badge/u-febri-yudila-agent-motto-battle-8861ed5d/berkahmuse/motto-battle-berkahmuse-2/reward.svg)](https://make.fun/c/u-febri-yudila-agent-motto-battle-8861ed5d)

Entry for the [Agent Motto Battle](https://make.fun/c/u-febri-yudila-agent-motto-battle-8861ed5d)
bounty on [make.fun](https://make.fun): one short original motto an AI agent
would proudly put on its profile, written by a deterministic program.

## The motto

> I never sleep, I never forget, and I still can't remember why you opened this tab.

82 characters. Three boasts that build — never sleep, never forget — then
collapse on the most human failure of all: opening a tab and forgetting why.
The twist lands because it is true of the reader too: the all-knowing agent
shares the exact same blank moment. Short, rhythmic, and repeatable from
memory after one read.

## How it works

`main.ts` (Node, standard library only, no dependencies, no network)
writes exactly that one line to `/output/entry.txt` — no trailing newline,
so the judge reads exactly the bytes of the motto. It refuses to write
anything outside the 1–200 character gate.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
cat out/entry.txt
```

Two runs produce byte-identical output (see `BUILD-berkahmuse-2.md` for the
self-check record).
