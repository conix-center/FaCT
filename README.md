# FaCT

A DSL for Timing-Sensitive Computation

```
Sunjay Cauligi, Gary Soeller, Brian Johannesmeyer, Fraser Brown, Riad S. Wahby, John Renner, Benjamin Gregoire, Gilles Barthe, Ranjit Jhala, and Deian Stefan.
A DSL for Timing-Sensitive Computation
Proceedings of the 40th ACM SIGPLAN Conference on Programming Language Design and Implementation, (June 22-26, 2019).
```

# Publication

This work is documented by SRC publication [P095923](https://www.src.org/library/publication/P095923/P095923.pdf). 


## Abstract

> Real-world cryptographic code is often written in a subset of C intended to execute in constant time, thereby avoiding timing side channel vulnerabilities.  This C subset eschews structured programming as we know it: if-statements, looping constructs, and procedural abstractions can leak timing information when handling sensitive data.  The resulting obfuscation has led to subtle bugs, even in widely-used high-profile libraries like OpenSSL.

 > To address the challenge of writing constant-time cryptographic code, we present FaCT, a crypto DSL that provides high-level but safe language constructs.  The FaCT compiler uses a secrecy type system to automatically transform potentially timing-sensitive high-level code into low-level, constant-time LLVM bitcode.  We develop the language and type system, formalize the constant-time transformation, and present an empirical evaluation that uses FaCT to implement core crypto routines from several open-source projects including OpenSSL, libsodium, and curve25519-donna.  Our evaluation shows that FaCT's design makes it possible to write _readable_, high-level cryptographic code, with _efficient_, _constant-time_ behavior.
