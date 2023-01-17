---
title: "Go Installation Guide"
author: William Burroughs
description: "A Go installation guide for Linux."
date: 2023-01-16T20:19:36-06:00
draft: false
---

# Go Installation Guide

## Linux 

### Installing Go with `apt`

1. Install the Go compiler.

```bash
sudo apt install gccgo
```

What is `gccgo`?
- Go compiler, based on the GCC back-end. This is the GNU Go compiler, which compiles Go on platforms supported by the gcc compiler. It uses the gcc backend to generate optimized code.
	
2. Install the `gc` compiler.

```bash
sudo apt install gccgo-go
```

What is `gccgo-go`?
- Go is a tool for managing Go source code (man `gccgo-go`).

**Note:** Recommended pkgs:
- `gcc-10-locales gcc-10-multilib gcc-10-doc gccgo-multilib gccgo-10-doc`


**Note:** If you're using _VIM_ with the ***coc***[^1] plugin, then install the Go extension with `:CocInstall coc-go`[^2] 

What is the difference between `gccgo` and `gc`(`gccgo-go`)?
- [Stack Overflow Answer](https://stackoverflow.com/questions/25811445/what-are-the-primary-differences-between-gc-and-gccgo)
- https://go.dev/blog/gccgo-in-gcc-471
- https://go.dev/doc/install/gccgo

### Usage

- Compiling a single file:

```bash
go build file.go
```

- Compiling a group:

1. Include `package file_name` at the beginning of Go script.
2. Execute: 

```Bash
go build
```

---

**Links**
- [[!Slipbox]]
- [[!Computer Science]]

## References
- https://go.dev/doc/install/gccgo 

[^1]: https://github.com/neoclide/coc.nvim
[^2]: https://github.com/josa42/coc-go
