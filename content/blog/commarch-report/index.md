---
title: Commarch
date: "2020-03-27"
description: "Commarch assignment report"
---

# React

React is a JavaScript library for building interfaces. It is the prevailing
front end library for the web. What sets React apart from previous options is
that it is simply a library for intelligently updating the dom (with some fancy
html style syntax if you want). React also encourages writing frontends in
terms of components through its api and JSX. React is backed by Facebook, but
as we'll see it's largely been the community that has been driving its
maintenance and evolution.

React was initially released May 29, 2013 and was originally authored by Jordan
Walke. In the frontend world, React can be considered a very mature project at
this point. While the project continually is improved with new features (Hooks,
and concurrent mode being the standouts) React is used in production systems by
countless businesses. React has had a major change to its DOM diffing, however
the API of React has been stable through this change. This sheds some light on
the fact that React has matured to the point that real caution is taken against
breaking changes.

React is an incredibly sustainable project. Not only is React supported by a
large organization that pays its employees to work on the project, it is also
supported by a community ranging from beginners and experienced professionals.
The fact that you can make a living teaching React to beginners speaks volumes
about how sustainable it is. Dan Abramov, a co creator of Redux, was brought on
to the React team at Facebook, which is a healthy sign that the React team is
receptive towards and values their community. Frontend technologies are a bit
driven by the idea of using the hottest new technology or library. React is
resilient towards losing out to hot new technologies as it is simply a library.
For example, while Angular may have a more cohesive API, and everything 'just
works', it's difficult for someone to come along and create something that
either improves or slots into the ecosystem.

React is MIT licensed, and is governed by Facebook employees. While Facebook
employees accept pull requests from the community, from the contribution graph
<https://github.com/facebook/react/graphs/contributors> we can see that almost
all of the top 50 contributors (by commits) are all or were Facebook employees.

# Zig

Zig is a programming language that can be thought of as a better C. Zig is to
Rust what Python is to Haskell. The project was started by Andrew Kelley in
2016\. He currently works full time on the project. It provides a way to write
fast programs that do not need certain safety guarantees. Basically, if you can
write C, you can write Zig, and once you do, you'll find you're not shooting
yourself in the foot as often. If you go from writing Rust to Zig, you'll find
that you're fighting with the compiler less often when you're using unsafe Rust
anyway.

Zig is not exactly mature. It is hard to find companies that use Zig in
production. It is also hard to find many community projects on GitHub that use
Zig. However when it comes to niche and in development programming languages,
Zig is quite popular. Zig was on the front page of Hacker News quite recently
<https://news.ycombinator.com/item?id=22679138>. For the conservative systems
programming ecosystem, Zig is one of the fastest growing projects on GitHub.
From my own experience playing with Zig the API is very fragile at the moment,
so I would not consider the project mature.

At the moment it's hard to say that Zig is sustainable. While the project has
been around since 2016, Andrew Kelley is by far its main contributor and
maintainer. Zig is not backed by any company and runs solely on a small
community of contributors towards Andrew's work. Zig sees surges in popularity
every few months it seems whenever it's posted on sites like Hacker News. I
don't see the project being sustained in this manner much longer however. It's
unlikely that the project will see a rapid surge in popularity such that it can
be self sustaining. Seeing as this is a systems level project it can actually
be quite sustainable so long as the slower growth in popularity keeps pace with
the systems programming ecosystem.

Zig is MIT licensed, and is largely governed by Andrew K. Andrew K has the last
word when it comes to what is contributed to the project. From my experiencing
contributing to Zig it is very lax when it comes to how and what you contribute
to, though this is likely only sustainable due to how early stage the project
is.

# Comparison

## Maturity

Clearly React is the more mature project, as it sees much more use in
production, and has been in development since 2011 under funding of one of the
largest corporations in the world. Zig has not even reached 1.0 and has a
brittle API. Although they were created for very different reasons and are a
part of ecosystems that move at a different pace, I think it's safe to say
React is the more mature project in this case.

## Sustainabiity

Again the difference here is pretty stark. React is backed by a huge company,
dedicated community, and has a cool factor among most younger programmers. Zig
on the other hand is largely maintained by a single significant contributor
whos only monetary form of support is through donations. What's impressive
about Zig in this regard is that it has gained many people's attention despite
being part of the systems programming ecosystem and without the backing of a
large company.

## Governance

Both React and Zig are MIT licensed and have a central form of governance.
React's own team decides what go in and out of the language, similar to Andrew
Kelley having the final say about Zig. React and Zig have different standards
for their contributors however. While Zig's contribution guideline are
basically to have some tests, React has quite a comprehensive guide
<https://reactjs.org/docs/how-to-contribute.html>.
