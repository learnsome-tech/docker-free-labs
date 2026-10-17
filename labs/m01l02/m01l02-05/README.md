# m01l02-05 · Control groups: the limit is a file

**Lesson:** [Namespaces And Cgroups: Isolation And Limits](https://learnsome.tech/learn/docker-course/m01l02) (lesson 1.2, module 1: Containers From The Ground Up) · Free  
**Check:** Read along

## Goal

You can name the kernel features that make a container, read a container's namespace identifiers and control group limits from a shell, and explain which of the two does isolation and which does resource control.

## Files

- [`starter/run.sh`](starter/run.sh): the command the lesson ran
- [`starter/session.sh`](starter/session.sh): the listing from the lesson
- [`starter/setup.sh`](starter/setup.sh)
- [`check.json`](check.json): how `./check` runs and checks this lab

## Steps

1. Read `starter/session.sh` alongside the lesson.
2. On a machine that has what it needs, the lesson ran it with:

   ```sh
   bash setup.sh >/dev/null 2>&1
   cg=/sys/fs/cgroup
   docker run --rm alpine:3.20 cat $cg/memory.max
   docker run --rm -m 64m alpine:3.20 cat $cg/memory.max
   docker run --rm --cpus=0.5 alpine:3.20 cat $cg/cpu.max
   docker run --rm --pids-limit=20 alpine:3.20 cat $cg/pids.max
   ```

## How to check

**Read along.** It needs Docker (or another container engine), which the lab sandbox does not have. Run it on a machine with Docker installed.

There is nothing to check: `./check m01l02-05` says so and moves on.

---

[Open the lesson on LearnSome.tech](https://learnsome.tech/learn/docker-course/m01l02) · [All labs of this lesson](../README.md) · [Course README](../../../README.md)
