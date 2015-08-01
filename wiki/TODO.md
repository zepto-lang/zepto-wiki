# TODO

There are a couple of features that are to be implemented at some point or another.
Here is a quick and dirty list of everything I have in mind ordered by informed guesses
about each points' scope:

**Small:**
* fix single number expression (in the repl 1.5lasd is parsed as 1.5)
* fix obscure single non-expression bug (triggered by e.g. `(begin (define x 10) (display "foo") x)` - parse error

**Medium:**
* Profiling shows getting variables(especially namespaced vars) takes ages(~86% of execution time). Fix that.
* Create byte vector type and http library
* Make macros more robust
* Fix continuations
* Make cl libraries work
* add traceback to errors
* add pattern matching

**Big:**
* Foreign Function Interface to C and Haskell
* Wrap OpenGL (https://github.com/haskell-opengl/OpenGL)
* A Compiler
  - with backend targetting gpu/ptx (maybe par-define?)
* A solid actor-based concurrency system (+ transactional memory)

