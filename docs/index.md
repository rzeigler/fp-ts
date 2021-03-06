---
title: Home
---

<img alt="fp-ts logo" src="./fp-ts-logo.png" style="display: block; width: 200px; margin-bottom: 2em;">

# Typed functional programming in TypeScript

fp-ts provides developers with popular patterns and reliable abstractions from typed functional languages in TypeScript.
{: .fs-6 .fw-300 }

[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [Take the tutorial](#tutorials){: .btn .fs-5 .mb-4 .mb-md-0 }

---

## Introduction

`fp-ts` includes the most popular data types, type classes, and abstractions such as `Option`, `Either`, `IO`, `Task`, `Functor`, `Applicative`, `Monad` to empower users to write pure FP apps and libraries built atop higher order abstractions.

A distinctive feature of `fp-ts` with respect to other functional libraries is its implementation of [Higher Kinded Types](<https://en.wikipedia.org/wiki/Kind_(type_theory)>), which TypeScript doesn't support natively. The idea for emulating higher kinded types in TypeScript is based on [Lightweight higher-kinded polymorphism](https://www.cl.cam.ac.uk/~jdy22/papers/lightweight-higher-kinded-polymorphism.pdf).

`fp-ts` takes inspiration from [Haskell](https://haskell-lang.org), [PureScript](http://www.purescript.org), and [Scala](https://www.scala-lang.org/), among others.

## Table of Contents

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Installation and TypeScript compatibility](#installation-and-typescript-compatibility)
- [Getting started](#getting-started)
- [Documentation](#documentation)
  - [Blog posts](#blog-posts)
  - [Tutorials](#tutorials)
- [Ecosystem](#ecosystem)
  - [Libraries](#libraries)
  - [Bindings](#bindings)
- [Type Classes Diagram](#type-classes-diagram)
- [License](#license)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Installation and TypeScript compatibility

To install the stable version:

```
npm install fp-ts
```

The stable version is tested against **TypeScript 3.3.3**, but should run with TypeScript 2.8.0+ too

**Note**. This library is conceived, tested and is supposed to be consumed by TypeScript with the `strict` flag turned on.

**Note**. If you are running `< typescript@3.0.1` you have to polyfill the `unknown` type. You can use [unknown-ts](https://github.com/gcanti/unknown-ts) as a polyfill.

**Note**. Make sure to always have a single version of `fp-ts` installed in your project. Multiple versions are known to cause `tsc` to hang during compilation. You can check the versions currently installed using `npm ls fp-ts` (make sure there's a single version and all the others are marked as `deduped`).

# Getting started

If you are coming from JavaScript:

- read [Mostly adequate guide to FP](https://github.com/MostlyAdequate/mostly-adequate-guide) by [@DrBoolean](https://github.com/DrBoolean)
- read this [blog series](http://www.tomharding.me/2017/03/03/fantas-eel-and-specification) on functional programming in JavaScript by Tom Harding, and then check out [the code](fantas-eel-and-specification) translated to TypeScript (there's a file for each blog post)

If you are using `ramda`

- [Comparison with ramda](https://github.com/gcanti/fp-ts/blob/master/ramda.md)

If you are coming from TypeScript:

- [How to write type class instances for your data structures](https://github.com/gcanti/fp-ts/blob/master/HKT.md)

If you are coming from Haskell or Purescript:

- [Comparison with PureScript](https://github.com/gcanti/fp-ts/blob/master/fp-ts-for-purescripters.md)

# Documentation

- [API Reference](https://github.com/gcanti/fp-ts/docs/index.md)

## Blog posts

- [Interoperability with non functional code using fp-ts](https://dev.to/gcanti/interoperability-with-non-functional-code-using-fp-ts-432e)
- [Functional design: combinators](https://dev.to/gcanti/functional-design-combinators-14pn)
- [Functional design: how to make the `time` combinator more general](https://dev.to/gcanti/functional-design-how-to-make-the-time-combinator-more-general-3fge)
- [Functional design: tagless final](https://dev.to/gcanti/functional-design-tagless-final-332k)

## Tutorials

**Beginner**

- [Debugging using the `Trace` module (code)](https://github.com/gcanti/fp-ts/blob/master/tutorials/debugging-with-Trace.ts)

**Advanced**

- [Free monad and `fp-ts` (code)](https://github.com/gcanti/fp-ts/blob/master/tutorials/Free.ts)
- [MTL-style in `fp-ts` (code)](https://github.com/gcanti/fp-ts/blob/master/examples/mtl.ts)
- [Type safe finite state machines with `IxIO` (code)](https://github.com/gcanti/fp-ts/blob/master/examples/ixIO.ts)

# Ecosystem

## Libraries

- [fp-ts-codegen](https://github.com/gcanti/fp-ts-codegen) - TypeScript code generation from a haskell-like syntax for ADT
- [io-ts](https://github.com/gcanti/io-ts) - TypeScript compatible runtime type system for IO validation
- [monocle-ts](https://github.com/gcanti/monocle-ts) - Functional optics: a (partial) porting of scala monocle to
  TypeScript
- [newtype-ts](https://github.com/gcanti/newtype-ts) - Implementation of newtypes in TypeScript
- [logging-ts](https://github.com/gcanti/logging-ts) - Composable loggers for TypeScript
- [fp-ts-routing](https://github.com/gcanti/fp-ts-routing) - A type-safe bidirectional routing library for TypeScript
- [parser-ts](https://github.com/gcanti/parser-ts) - String parser combinators for TypeScript
- [remote-data-ts](https://github.com/devex-web-frontend/remote-data-ts) - RemoteData type (check [this article](https://medium.com/@gcanti/slaying-a-ui-antipattern-with-flow-5eed0cfb627b))
- [retry-ts](https://github.com/gcanti/retry-ts) - Retry combinators for monadic actions that may fail
- [fp-ts-local-storage](https://github.com/gcanti/fp-ts-local-storage) - fp-ts bindings for LocalStorage
- [circuit-breaker-monad](https://github.com/YBogomolov/circuit-breaker-monad) - Circuit Breaker pattern as a monad

## Bindings

- [fp-ts-rxjs](https://github.com/gcanti/fp-ts-rxjs) - fp-ts bindings for RxJS
- [fp-ts-fluture](https://github.com/gcanti/fp-ts-fluture) - fp-ts bindings for Fluture
- [fp-ts-most](https://github.com/joshburgess/fp-ts-most) - fp-ts bindings for @most/core

# License

The MIT License (MIT)
