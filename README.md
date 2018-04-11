:construction: **I'm still working on finalizing the keyboard layout and adding configuration files.** [Here's a spreadsheet of the current plan.](https://docs.google.com/spreadsheets/d/1GyCh6h8Ttc9uhrkitXT-BJbw4bowhrKhP1Uw25iINrk/edit) :construction:

# alt-vim-keys

This is a collection of keybindings for Vi/Vim and Vim emulators (particularly [atom-vim-mode-plus](https://github.com/t9md/atom-vim-mode-plus) for [Atom](https://atom.io/))

**This project is for:**
- People who use Vim on keyboard layouts other than Qwerty and want a set of keybinds that stays in the same place
- People looking to capture the power of Vim without learning keybinds based on a decades-old keyboard that nobody uses any more

**This project is not for:**
- Sysadmins or people who are frequently accessing other computers that have vanilla Vim
- People who are already used to vanilla Vim or like hjkl movement

## Goals

* Keys that are often repeated (e.g. scrolling) should use modifiers and not leader keys
* Related keys (e.g. insert/append) should be spatially related
* Movement keys should generally be assigned to the right hand, and commands/operators to the left
  - If a user likes to use the mouse sometimes, it is easier to start a command with the left hand while transitioning the right hand to the keyboard
  - This also gives a sense of coherency to the layout
* Infrequently-used actions (e.g. reflow paragraph) should require leader and/or modifier keys
  - If a user wants some of these actions to be easier to perform, they can configure some of the available key combinations as needed

## Highlights

Here are some major features of the keymap (here using Qwerty):

- `ijkl` for basic movement
- `zxcv` for undo/redo, cut (`delete`), copy (`yank`), paste (`put`)
- `ctrl-;` to access normal mode (slightly easier than `ctrl-[`)
- `;` and `p` are the primary leader keys
- favors usage of leader key over repeated keys
- `df` for `insert` and `append`
- `um` for scrolling up/down
- `yhn` for `redraw-cursor-line-at-…` and `move-to-…-of-screen`
- tab key is for indentation
- `s` for select (`activate-visual-mode`); pressing `s` again cycles through characterwise, linewise, and blockwise visual modes
- `,.` for `till-backwards` and `till` (hold shift for `find`)
- `\|` for `mark` and `move-to-mark`
- pane navigation/movement
- includes keybinds for [atom-narrow](https://github.com/t9md/atom-narrow)
