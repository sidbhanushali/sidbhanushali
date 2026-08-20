# Sid Bhanushali

Building RL training environments for production incidents.

I've spent the last five years running hardened Kubernetes platforms in
regulated, air-gapped environments. GitLab pipelines, ArgoCD, and all the ways
they break at 2am. Almost none of that work is public. This is the public half.

## What I'm working on

Frontier models still fail most Kubernetes incident tasks on public
leaderboards, and part of the problem is there's barely anything to train them
on. You need containerized worlds that are broken the way real prod breaks
(actual root causes, not a chaos tool flipping bits), graded by checks that ask
whether the system is actually healthy again instead of whether the alert went
quiet.

So I'm building those.

Areas I care about:
- Infra incidents: cascading cert failures, OOM spirals, compound faults that
  stay broken after the trigger is gone
- Security incidents (defensive IR only): RBAC lockouts, secret rotation gone
  wrong, poisoned images
- Oracle design: graders that can't be reward-hacked, negative checks,
  environments that survive 1,000 parallel runs

Right now: working through the [SREGym](https://github.com/SREGym/SREGym)
codebase and building scenarios for it.
