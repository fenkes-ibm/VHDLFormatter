# VHDL Fomatter

VHDL formatter web online written in javascript

[Online version https://g2384.github.io/VHDLFormatter/](https://g2384.github.io/VHDLFormatter/)

## Release Notes

### 2.7 [2020-10-19]

- align concurrent signal assignment
- align in, out, buffer and inout key words
- fix single line PACKAGE indentation
- add more type names, support "STD_LOGIC", "STD_LOGIC_VECTOR", "STD_ULOGIC", "STD_ULOGIC_VECTOR"
- add new lines at the end of file
- update packages

### 2.6 [2020-02-23]

- support VHDL-2008 block comment /* */
- use jest
- indent multi-line signal and constant declarations
- do not add space between "<" or ">"; e.g. "<<<" will become " <<< " and not " < < < "
- array type definition breaks when formatting; e.g. "RANGE <>" becomes "RANGE < >"

### 2.5 [2019-03-13]

- keep the front page concise
- add `style.css`, improve UI
- support all browsers (do not use `RegExp Lookbehind Assertions`)

### 2.4 [2019-02-23]

- use local storage to store settings
- add `main.js`
- treat key words and type names separately
- expand/hide setting options
- align signs locally or globally

### 2.3 [2019-02-22]

- bugfix "remove non-comment code by mistake"
- add `tests` folder, improve the project management
- support extended identifier (backslash names)
- fix exponential notation
- user can choose EOL symbols (or use system's by default)
- align comments (when user chooses "align" option)
- bugfix "extra whitespaces around unary minus or plus"

Many thanks to [@MihaiBabiac](https://github.com/MihaiBabiac)

### 2.2 [2018-10-16]

- support enumerated types

### 2.1 [2018-03-22]

- fix keywords case issues
- anything in quotes will not be touched
- correct format for comments after multi-line statement
- options to align signs in parameter lists
- fix function indentation
- fix "align symbols affects process label"
- do not align multi-occurrence symbols in a line
- better styles (checkbox, button, disabled)
- support package bodies
- fix "newline after PORT affects PORT MAP"

### 2.0 [2018-02-16]

- rewrite the main algorithm (& move to a new repository)
- add more unit tests
- fix all known issues

### 1.1 [2016-11]

- fix some bugs reported by users
- add unit tests

### 1.0 [2015-01]

- support most of the VHDL features