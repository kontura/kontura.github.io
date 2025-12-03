---
title: "Tiler (Odin, WASM, Raylib)"
---

![rockquid](/tiler.png)

[Repository](https://github.com/kontura/tiler)

Available at https://tiler.kontura.cc/

This is a peer to peer tool for simple rpg battle maps.

It uses odin and raylib to generate a grid of tiles. Each tile can have several different attributes like color, tokens, walls etc..

It is compiled to WASM using [emscripten](https://emscripten.org/) and runs in the browser.

It is a local first application, peers synchronize a list of actions.

Each peer first connects to a simple Python signaling server using a websocket after it learns about other peers it attempts
to connect to each other peer using [WebRTC](https://webrtc.org/). If it fails it keeps synchronizing via the signaling server.
