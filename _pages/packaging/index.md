---
title: Team Packaging Guide
layout: page
permalink: "/packaging/"
---

## Team Packaging Guide

### Adding a package

If you want to make an existing package in Debian to be team-maintained by
the Debian Chinese Team, please send an email to [Team Alioth Maillist](mailto:chinese-developers@lists.alioth.debian.org)
and explain your reason.

If you find an new interesting package and want to make it team-maintained
from the beginning, please follow the regular ITP process first. Meanwhile,
please also send an email to the maillist about your initiative.

#### Acceptance Guideline

The team will most likely accept Chinese-related packages into the team.
If you are in doubt, please get into contact with us.

### Maintaining packages

#### Workflow

We use Git to manage team packages. You are recommended to follow
[DEP-14](http://dep.debian.net/deps/dep14/) to make the Git repository
canonical.

* [Team Git Repository Overview](https://anonscm.debian.org/git/chinese/)

#### Rules and Hints

* Use CLI tool provided by Alioth to set up new repository.
* Use **annotated tags** for Git. This is mandatory as written inside Git hook.
* Tags cannot be removed from remote, so be careful. If things go wrong, you will have to operate manually on Alioth host.
* All new commits will trigger an email onto [chinese-commits](mailto:chinese-commits@lists.alioth.debian.org) as written inside Git hook.
* Be responsive to team members, and always send an email into the maillist to explain what you are doing before touching others' package inside the team.
