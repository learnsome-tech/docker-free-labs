# m01l01-03 · A container is a process, not a machine

**Lesson:** [Why Containers: Bare Metal, Machines And Processes](https://learnsome.tech/learn/docker-course/m01l01) (lesson 1.1, module 1: Containers From The Ground Up) · Free  
**Check:** Read along

## Goal

You can explain what a container actually is, how it differs from a virtual machine, and why packaging the environment with the program removes a whole class of deployment failure.

## Files

- [`starter/run.sh`](starter/run.sh): the command the lesson ran
- [`starter/session.sh`](starter/session.sh): the listing from the lesson
- [`check.json`](check.json): how `./check` runs and checks this lab

## Steps

1. Read `starter/session.sh` alongside the lesson.
2. On a machine that has what it needs, the lesson ran it with:

   ```sh
   docker run --rm alpine:3.20 ps -o pid,comm
   docker run --rm alpine:3.20 sh -c 'echo hello from inside'
   ```

## How to check

**Read along.** It needs Docker (or another container engine), which the lab sandbox does not have. Run it on a machine with Docker installed.

There is nothing to check: `./check m01l01-03` says so and moves on.

---

[Open the lesson on LearnSome.tech](https://learnsome.tech/learn/docker-course/m01l01) · [All labs of this lesson](../README.md) · [Course README](../../../README.md)
