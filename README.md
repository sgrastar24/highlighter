# hl

This script highlights texts that matches the given pattern so make text that you want to find easier to see.

## Examples

Suppose you are monitoring web server logs.
If you want to find a particular string, simply specify that string as an argument.

![Example1](img/example1.gif)

Regular expressions can be used for patterns.
Attributes such as underline can also be used if the terminal supports it.

An example where you do not want to mind lines with a response status of 2XX/3XX.

![Example2](img/example2.gif)


## Usage

```
hl [options] PATTERN FILE...
hl [options] [-e PATTERN | -f FILE] [FILE...]
| hl PATTERN

  -a, --attribute=<ATTRIBUTE>[,<ATTRIBUTE...>]
            use ATTRIBUTEs when print matching PATTERN
            allow the ATTRIBUTEs to be abbreviated to uniqueness
  -x, --fixed       interpret PATTERN as a fixed string
  -w, --word-regexp force PATTERN to match only whole words
  -i, --ignore-case ignore case distinctions
  -l, --line        apply the attributes whole line matching PATTERN
  -e, --regexp=PATTERN  use PATTERN as a regular expression
  -f, --file=FILE   obtain PATTERN from FILE
  -g, --grep        show only the line matching PATTERN as 'grep --color'
  -h, --help        display this help and exit
```

Attributes | Specifiable parameters
--- | ---
Foreground colors | black, red, green, yellow, blue, magenta, cyan, white
Background colors | on_black, on_red, on_green, on_yellow, on_blue, on_magenta, on_cyan, on_white
Styles | bold, dark, underline, blink, reverse, concealed


