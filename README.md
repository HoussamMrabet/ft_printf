# ft_printf

[![SUCCESS](https://i.postimg.cc/cH23NFHK/Screen-Shot-2023-12-03-at-9-50-07-AM.png)](https://postimg.cc/0MGjYd7x)

## Because ft_putnbr() and ft_putstr() aren’t enough

### Summary:

The goal of this project is to recode `printf()`, a popular and versatile C function. By doing so, you will primarily learn about using a variable number of arguments. How cool is that? Well, it's actually pretty cool :)

### Version: 10

## Contents

I. [Introduction](#introduction)  
II. [Common Instructions](#common-instructions)  
III. [Mandatory Part](#mandatory-part)  
IV. [Bonus Part](#bonus-part)  
V. [Submission and Peer-evaluation](#submission-and-peer-evaluation)

## Chapter I: Introduction

In this project, you will delve into the implementation of a well-known C function - `printf()`. This exercise offers a great opportunity to enhance your programming skills, especially in dealing with variadic functions in C. The key to success lies in crafting a well-structured and extensible code.

Upon completing this assignment, you will have the privilege of incorporating your `ft_printf()` into your `libft`, enabling its use in your future C projects at school.

## Chapter II: Common Instructions

- Your project must be written in C.
- Adhere to the Norm. Bonus files/functions are included in the norm check.
- Functions should not quit unexpectedly (segmentation fault, bus error, double free, etc.), except for undefined behaviors.
- Free all heap-allocated memory properly; no leaks will be tolerated.
- If a Makefile is required, include one that compiles with `-Wall`, `-Wextra`, and `-Werror` flags, using `cc`.
- Include rules in your Makefile for `$(NAME)`, `all`, `clean`, `fclean`, and `re`.
- For bonuses, add a `bonus` rule to your Makefile, and forbidden components must be in a separate file `_bonus.{c/h}`.
- If your project uses `libft`, copy its sources and Makefile to a `libft` folder, and your project's Makefile should compile the library using its Makefile.
- Create test programs for your project, though they won't be submitted; they'll be helpful during defense.

## Chapter III: Mandatory Part

### Program name: libftprintf.a
### Turn in files: Makefile, *.h, */*.h, *.c, */*.c
### Makefile rules: `NAME`, `all`, `clean`, `fclean`, `re`
### External functions: `malloc`, `free`, `write`, `va_start`, `va_arg`, `va_copy`, `va_end`
### Libft authorized: Yes

Description: Write a library that contains `ft_printf()`, a function mimicking the original `printf()`. The prototype of `ft_printf()` is:

```c
int ft_printf(const char *, ...);
```

Requirements:

- Do not implement the buffer management of the original `printf()`.
- Handle the following conversions: `cspdiuxX%`.
- Your function will be compared against the original `printf()`.
- Use the `ar` command to create your library; using `libtool` is forbidden.
- Create `libftprintf.a` at the root of your repository.

## Chapter IV: Bonus Part

You don't have to do all the bonuses. The bonus part will only be assessed if the mandatory part is perfect. If the mandatory part has not been completed perfectly, the bonus part will not be evaluated.

Bonus list:

- Manage any combination of the flags: `'-' '0.'` and the field minimum width under all conversions.
- Manage all the following flags: `'# +'` (Yes, one of them is a space).

If you plan to complete the bonus part, consider implementing your extra features from the start to avoid the pitfalls of a naive approach.

## Chapter V: Submission and Peer-evaluation

Turn in your assignment in your Git repository as usual. Only the work inside your repository will be evaluated during the defense. Double-check the names of your files to ensure correctness.

Upon successful completion of this assignment, you are allowed to add your `ft_printf()` to your `libft` for use in your school C projects.
