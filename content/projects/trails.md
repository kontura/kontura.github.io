---
title: "Trails (Lua, Neovim)"
---

![trails](/trails.png)

[Repository](https://github.com/kontura/trails.nvim)

Neovim plugin generating interactive ascii art call graph.

Inspired by now archived [Sourcetrail](https://github.com/CoatiSoftware/Sourcetrail).

Requires set up LSP because it is using `callHierarchy/incomingCalls` handler to get the required information.

It is using a simple genetic algorithm to minimize the number of crossings in the generated graph.
