# SublimeYardoc

Package for Sublime Text 3.

This is a fork of the original [sublime-yardoc](https://github.com/revathskumar/sublime-yardoc) with some my improvements.

## Install

**Via Package Control**:

1. Open Command Palette &rarr; `Package Control: Add Repository` &rarr; `https://github.com/phts/SublimeYardoc`
2. Open Command Palette &rarr; `Package Control: Install Package` &rarr; `SublimeYardoc`

## Usage

Pressing **ctrl+enter** on the line of the method definition
```ruby
def hello a, b

end
```

results

```ruby
#
# [hello description]
# @param a [type] [description]
# @param b [type] [description]
#
# @return [type] [description]
def hello a, b

end
```

![Method yardoc](https://lh6.googleusercontent.com/-C9V-e0vzDq0/UERyoS0I4oI/AAAAAAAAG48/M2cptkMfmgA/s458/123.gif)

Pressing **ctrl+enter** on the line of the class definition

```ruby
class Hello

end
```

results

```ruby
#
# [class description]
#
# @author
#
class Hello

end
```

## Settings

```json
// Determines if empty comment lines have a trailing space
"trailing_spaces": true,

// Add an initial empty line at the beginning of the comment
"initial_empty_line": true,

// Add an empty line at the end of the comment
"trailing_empty_line": false,
```
