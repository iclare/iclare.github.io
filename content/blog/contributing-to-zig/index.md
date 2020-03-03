---
title: Zig
date: "2020-03-03"
description: "My experience contributing to Zig."
---

I heard about the [Zig](https://ziglang.org/) programming language, about a
year ago. In short, Zig is a high performance language with tight C integration
that values simplicity, explicitness, and control. I've always been interested
in high performance and low level programming, so Zig caught my interest. What
I also like about Zig is that you do not need to learn and use additional
syntax or keywords, or shift your programming style to convince the language
that you know what you're doing [Unsafe Zig is Safer than Unsafe](https://andrewkelley.me/post/unsafe-zig-safer-than-unsafe-rust.html).

With Zig, the priority is not just to have a safer language, but also
to be a small simple language that has no hidden control flow. All control flow
is made explicit in Zig. Zig also gives you full control over memory, as well
as making it obvious when anything is going to allocate memory. Zig allows you
to create your own allocators [manual memory management](https://ziglang.org/#toc-Manual-memory-management).

While Zig may be an easy language to learn (with just a 500 line file
describing its grammar, [Grammar file](https://ziglang.org/documentation/master/#Grammar))
the project is still changing at a fast pace. the last major release `0.5.0`
came just a few months after the previous major release.

Zig doesn't try to compete with languages like Rust or C++, instead it is meant
to compete with C, and takes advantage of its ecosystem. Among other C related features,
Zig also ships with ability to translate C into Zig.

Zig's community is another reason why I took interest in the language.
Zig was created by [Andrew Kelley](https://andrewkelley.me/).
He works on Zig full time and interacts frequently with the [community](https://github.com/ziglang/zig/wiki/Community),
you'll usually see him answering question on the IRC, or working on Zig
on his [Twitch channel](https://www.twitch.tv/andrewrok).
Zig is pretty open to contribution, and has a receptive community.
Zig's [CONTRIBUTING.md](https://github.com/ziglang/zig/blob/master/CONTRIBUTING.md)
basically has no restrictions other than suggesting you add a test case for
your changes.

I wanted to learn Zig and get involved in the community so I looked into open
issues that were labeled contributor friendly.

I ended up submitting a WIP PR related to the C to Zig translation feature.

[WIP Detect number literals from macro substitution](https://github.com/ziglang/zig/pull/4604)

I wasn't able to completely address the issue I was fixing, although it seemed
pretty simple on the surface, it actually took quite a bit of time setting up
Zig, and reading the code that was already there. Zig is wrapping clang's AST
API, but did not include the functions I needed to be able to detect whether an
integer literal came from a macro substitution, so I had to do some reading of
the clang API as well.

In retrospect I was probably way too ambitious taking this on considering how
hard my current semester in school has been, but I wanted a fun challenge. Thankfully, the
Zig creator architects his code so that it is easy to contribute to the
higher level aspects of the project.

I actually had quite a bit more code than what I submitted in the pull request,
but I realized I was making pretty big assumptions, and probably should submit
what I already had just to make sure I was heading in the right direction.

In the pull request at the moment, while I'm able to determine that an integer
literal came from a macro, I do not yet get the name of the macro and
substitute that in place of the integer literal. I wrote a solution which
unfortunately depended on clang/lexer, which is not used anywhere else in the
project, so I decided so rip that out and ask for feedback on what I had up to
detecting int literal macros.

I hope to gain some feedback soon. Be on the look out for part 2 of this post if this interested you.

