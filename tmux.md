# tmux

General ideas

* Use standard key binding to be familiar with default installation on foreign systems.
* No-nonsense - Focus on stuff that I really use (highly subjective).
* Organize by topic
* Wording based on [tmux(1) — Linux manual page]

## Key Bindings

### Panes

Create & Navigate

* `C-B "` - Split the current pane into two, top and bottom.
* `C-B %` - Split the current pane into two, left and right.
* `C-B o` - Select the next pane in the current window.
* `C-B &` - Kill the current window.
* `C-B [up|down|left|right]` - Change pane current pane.

Resize & Swap

* `C-B C-[up|down|left|right])` - Resize the current pane in steps of one cell.
* `C-B M-[up|down|left|right]` - Resize the current pane in steps of five cells.
* `C-B {` - Swap the current pane with the previous pane.
* `C-B }` - Swap the current pane with the next pane.
* `C-B z` - Toggle zoom state of the current pane.

### Copy & Paste

* `C-B [` - Enter copy mode to copy text or view the history.
* `C-B ]` - Paste the most recently copied buffer of text.

### Misc

* `C-b d` - key strokes
* `C-b ?` - List all key bindings.
* `C-b d` - Detach the current client.

### All


## Command Line Parameters

### Reattach

Each session is persistent and will survive accidental disconnection or intentional detaching (with the ‘C-b d’ key strokes) may be reattached using:

```sh
tmux attach
```

## References

* [tmux(1) — Linux manual page]

[tmux(1) — Linux manual page]: https://man7.org/linux/man-pages/man1/tmux.1.html

<!-- 
Unused to later additions (see man tmux)

C-o         Rotate the panes in the current window forwards.
!           Break the current pane out of the window.
#           List all paste buffers.
$           Rename the current session.
&           Kill the current window.
'           Prompt for a window index to select.
(           Switch the attached client to the previous session.
)           Switch the attached client to the next session.
,           Rename the current window.
-           Delete the most recently copied buffer of text.
.           Prompt for an index to move the current window.
0 to 9      Select windows 0 to 9.
:           Enter the command prompt.
;           Move to the previously active pane.
=           Choose which buffer to paste interactively from a list.
c           Create a new window.
f           Prompt to search for text in open windows.
i           Display some information about the current window.
l           Move to the previously selected window.
m           Mark the current pane (see select-pane -m).
M           Clear the marked pane.
n           Change to the next window.
o           Select the next pane in the current window.
p           Change to the previous window.
q           Briefly display pane indexes.
r           Force redraw of the attached client.
s           Select a new session for the attached client interactively.
w           Choose the current window interactively.
x           Kill the current pane.
~           Show previous messages from , if any.
Page Up     Enter copy mode and scroll one page up.
M-1 to M-5  Arrange panes in one of the five preset
            layouts: even-horizontal, even-vertical, main-
            horizontal, main-vertical, or tiled.
Space       Arrange the current window in the next preset layout.
M-n         Move to the next window with a bell or activity marker.
M-o         Rotate the panes in the current window backwards.
M-p         Move to the previous window with a bell or activity marker.
-->
