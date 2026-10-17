# m01l05-02 · Installing the engine on a Debian or Ubuntu host

**Lesson:** [Install Docker And Verify Your Environment](https://learnsome.tech/learn/docker-course/m01l05) (lesson 1.5, module 1: Containers From The Ground Up) · Free  
**Check:** Read along

## Goal

You can install the right Docker for your operating system, prove the daemon is reachable from your shell, and know which post-install steps decide whether you type sudo for the rest of your career.

## Files

- [`starter/install-docker.sh`](starter/install-docker.sh): the listing from the lesson
- [`check.json`](check.json): how `./check` runs and checks this lab

## Steps

1. Read `starter/install-docker.sh` alongside the lesson.
2. Follow it the way the lesson builds it:
   - Lines 1–5: the convenience script
   - Lines 6–9: adds you to the docker group
   - Lines 10–12: enables the service
   - Lines 13–15: proves the whole path
3. Notes from the lesson:
   - Line 5: fine for a disposable machine; use the repository on a real server
   - Line 8: membership of this group is equivalent to root on the host

## How to check

**Read along.** It is a listing to read alongside the lesson, not a program to run.

There is nothing to check: `./check m01l05-02` says so and moves on.

---

[Open the lesson on LearnSome.tech](https://learnsome.tech/learn/docker-course/m01l05) · [All labs of this lesson](../README.md) · [Course README](../../../README.md)
