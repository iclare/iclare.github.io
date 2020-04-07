---
title: WebAssembly
date: "2020-02-26"
description: "Run native code in the browser."
---

WebAssembly is a low level language that runs with
near-native performance. It is not intended to be written by hand,
and so provides a compilation target for languages like C/C++ and Rust.
This means these languages now have a way to run on the web.

# So What?

The implications of WebAssembly are pretty big.
WebAssembly means you can run code written
in any number of languages, on the web, at near native speed.

WebAssembly provides JavaScript APIs so you can load WebAssembly
modules into a JavaScript app. This means you can
replace parts of your code written in JavaScript with code
that targets WebAssembly, for massive performance gains.

WebAssembly is being developed as a web standard via W3C and the community groups. WebAssembly 1.0 has already shipped in Firefox, Chrome, Safari, and Edge.

# How does it work?

WebAssembly fits into a web platform that comes with web browsers.
In this web platform, there's a virtual machine that runs web app code
(JavaScript), and there's a set of APIs that can be called to control
the web platform; APIs like DOM, CSSOM, WebGL.

In the past, the VM of web platforms has only been able to load JavaScript.
While JavaScript works well for most problems on the web, certain applications, like 3D games, VR, AR, image/video editing demand greater performance than an interpreted language can provide.

Another issue is that browsers need to receive the full JavaScript source
of a web app in order to load it. This means large downloads, and on the fly
compilation that results in stuttering.

The small binary and ahead of time compilation of a WebAssembly module
results in web apps that are much faster to download and run with better
performance.

# How do I get started?

WebAssembly is still a young technology, so garbage collected languages
are not yet supported. Your best options are to either port a C/C++ application with Emscripten, Write a Rust application targeting WebAssembly as the output, or use AssemblyScript to write TypeScript style code that compiles to a WebAssembly binary. See the links below to get started with either of these options.

# See also

[webassembly.org](https://webassembly.org/)

[developer.mozilla.org/en-US/docs/WebAssembly/Concepts](https://developer.mozilla.org/en-US/docs/WebAssembly/Concepts)

[emscripten.org/docs/getting_started](https://emscripten.org/docs/getting_started/index.html)

[developer.mozilla.org/en-US/docs/WebAssembly/Rust_to_wasm](https://developer.mozilla.org/en-US/docs/WebAssembly/Rust_to_wasm)

[docs.assemblyscript.org](https://docs.assemblyscript.org/)
