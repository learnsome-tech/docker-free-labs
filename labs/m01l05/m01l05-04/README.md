# m01l05-04 · The canonical first container

**Lesson:** [Install Docker And Verify Your Environment](https://learnsome.tech/learn/docker-course/m01l05) (lesson 1.5, module 1: Containers From The Ground Up) · Free  
**Check:** Read along

## Goal

You can install the right Docker for your operating system, prove the daemon is reachable from your shell, and know which post-install steps decide whether you type sudo for the rest of your career.

## Files

- [`starter/install-docker.sh`](starter/install-docker.sh)
- [`starter/run.sh`](starter/run.sh): the command the lesson ran
- [`starter/session.sh`](starter/session.sh): the listing from the lesson
- [`starter/setup.sh`](starter/setup.sh)
- [`check.json`](check.json): how `./check` runs and checks this lab

## Steps

1. Read `starter/session.sh` alongside the lesson.
2. On a machine that has what it needs, the lesson ran it with:

   ```sh
   bash setup.sh >/dev/null 2>&1
   docker run --rm hello-world
   docker run --rm alpine:3.20 uname -m
   ```

## How to check

**Read along.** It needs Docker (or another container engine), which the lab sandbox does not have. Run it on a machine with Docker installed.

There is nothing to check: `./check m01l05-04` says so and moves on.

---

[Open the lesson on LearnSome.tech](https://learnsome.tech/learn/docker-course/m01l05) · [All labs of this lesson](../README.md) · [Course README](../../../README.md)
