# Console Graphing Calculator

A command-shell style graphing calculator that runs in the terminal. Function parameters are set with named commands. The current function can be graphed as ASCII output or analyzed with computed statistics.

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

---

## Interface

The program runs as a persistent command shell, styled after a DOS-style prompt, rather than a linear sequence of questions.

```
C:\Users\mathisjean> help

Available commands:
 A:           Set the value for 'a' slope or vertical stretch.
 B:           Set the value for 'B' exponential base or 'b' linear y-intercept.
 CLS:         Clears the terminal screen.
 DESCRIPTION: Displays information about the graphing calculator program.
 FUNCTION:    Choose and set a function.
 GRAPH:       Displays the graph of the current function.
 H:           Set the value for 'h' horizontal shift.
 HELP:        Shows this list of available commands.
 K:           Set the value for 'k' vertical shift.
 M:           Set the value for 'm' slope for linear function.
 R:           Set the value for 'r' radius for circles.
 RESET:       Resets all function variables to default values.
 STATISTICS:  Displays the equation, domain, image, and zeros of the function.

C:\Users\mathisjean> A

Select a value for 'a':
> 5

'a' has been set to 5
```

## Supported functions

- Linear functions, parameterized by `m` and `b`
- Exponential functions, parameterized by `a`, `B`, `h`, and `k`
- Circles, parameterized by `r`

Function type is selected with `FUNCTION`.

## Commands

| Command | Function |
|---|---|
| `A`, `B`, `H`, `K`, `M`, `R` | Set the corresponding function parameter |
| `FUNCTION` | Select the active function type |
| `GRAPH` | Renders the current function as an ASCII grid |
| `STATISTICS` | Computes and displays the equation, domain, image, and zeros of the current function |
| `RESET` | Resets all function variables to default values |
| `CLS` | Clears the terminal screen |
| `DESCRIPTION` | Displays information about the program |
| `HELP` | Lists available commands |

## Implementation

`GRAPH` output is generated from a two-dimensional array, with characters placed to trace the function's shape across a fixed grid. No graphics library is used.

This calculator runs [here](https://mathisjean.github.io/console_graphing_calculator/).

---

Terminal-based. No external dependencies.
