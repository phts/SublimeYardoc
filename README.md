## SublimeText package for generating Yardoc

This is a fork of the original [sublime-yardoc](https://github.com/revathskumar/sublime-yardoc) with some my improvements.

---

### Installation

- In Command Palette (ctrl+shift+p or cmd+shift+p) select: `Package Control: Add Repository`
  - Add this project's GitHub URL: https://github.com/phts/sublime-yardoc

- In the Command Palette, select: `Package Control: Install Package`
  - Search for `sublime-yardoc` and ensure the source references this repository

### Usage

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

### Settings

Two settings are available:

```json
    // Determines if empty comment lines have a trailing space
    "trailing_spaces": false,
    // Add an initial empty line at the beginning of the comment
    "initial_empty_line": false
```
```
