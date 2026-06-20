# ma2-parser

An `.ma2` to simai converter, the reverse companion to [maidata-parser](https://github.com/lcebot/maidata-parser).

**Download the latest binary from [Releases](https://github.com/lcebot/ma2-parser/releases/latest).**

---

## Overview

ma2-parser reads a `.ma2` chart file and outputs the equivalent simai notation to stdout.

---

## Download

Pre-built binaries are published on the [Releases](https://github.com/lcebot/ma2-parser/releases/latest) page.

---

## Usage

```
ma2_parser <input.ma2> [> output.txt]
```

The input must be a `.ma2` file with standard tab-separated fields. The simai output is written to stdout and can be redirected to a file or piped directly.

**Examples**

```sh
# Print simai to terminal
./ma2_parser chart.ma2

# Save to a file
./ma2_parser chart.ma2 > chart_inote.txt

# Pipe into another tool
./ma2_parser chart.ma2 | clip
```

**Options**

| Argument         | Description                                 |
| ---------------- | ------------------------------------------- |
| `<input.ma2>`    | *(required)* Path to the input `.ma2` file  |

There are no additional flags. Output always goes to stdout; redirect with `>` to write to a file.

---

## Notes

- This repository distributes compiled binaries only.
- The binary is self-contained and has no runtime dependencies.
