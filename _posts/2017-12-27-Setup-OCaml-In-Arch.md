---
layout: post
title:  "Setup OCaml in Manjaro"
date:   2017-12-27 06:19:38 +0800
categories: jekyll update
---

# Install

```
$ sudo pacman -S ocaml opam
```

# OPAM configuration

```
$ opam init -a -y --use-internal-solver
$ opam switch -y 4.05.0 --use-internal-solver
$ eval `opam config env`
$ opam install -y utop ounit qtest yojson lwt menhir ansiterminal lambda-term merlin ocp-indent user-setup bisect --use-internal-solver
$ opam user-setup install
```