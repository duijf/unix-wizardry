# Wizardry of the UNIX kind

This repo contains random bits of configuration and utilities that people have
asked me about. Maybe there's something in here that's useful to you. No
guarantees, however.

Feel free to open issues if you encounter trouble. I'll try to help, or maybe
someone else can.

## A Makefile for LaTeX documents

[Get it here.][latex-makefile]

The common wisdom is that you shouldn't use Makefiles for LaTeX builds. You
aren't going to get it right. That's true. Therefore, this one uses
[`latexrun`][latexrun] to handle the multitude of edge cases.

If there is a build tool that just does this, then why the Makefile? It strings
together some related tools that you'll probably try to get working. It'll also
save you some typing.

Probably won't work out of the box. Quite possibly, you need to know about
Makefiles to get this working.

Features:

 - Watch mode
 - Refresh `mupdf`
 - Multiple documents

Dependencies:

 - `latexrun`
 - `mupdf` (can be edited out)
 - `entr`
 - A LaTeX distribution

 [latexrun]:https://github.com/aclements/latexrun
 [latex-makefile]:./latex-makefile/Makefile
