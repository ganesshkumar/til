---
description: tmux cheatsheet
---

# Sessions

|Description|Command|
|:--|:--|
|Create a new session | tmux new -s session-name |
|Rename current session | `Ctrl-b` $ |
|List all running sessions | tmux ls <br> `Ctr-b` s |
|Detach from a session | tmux detach <br> `Ctrl-b` d |
|Attach to a session | tmux a -t session-name |
|Kill a session | tmux kill-session -t session-name |

# Windows

|Description|Command|
|:--|:--|
|Create a new window | `Ctrl-b` c|
|Rename current window | `Ctrl-b` ,|
|List all windows in current session | `Ctrl-b` w|
|Change to next window | `Ctrl-b` n|
|Change to previous window | `Ctrl-b` p|
|Select a particular window | `Ctrl-b` [0-9]|

# Panes

|Description|Command|
|:--|:--|
|Horizontally split current pane | `Ctrl-b` "|
|Vertically split current panes | `Ctrl-b` %|
|Show pane numbers | `Ctrl-b` q|
|Toggle between panes | `Ctrl-b` o|
|Swap with next pane | `Ctrl-b` }|
|Swap with previous pane | `Ctrl-b` {|
|Break the pane out of the window | `Ctrl-b` !|
|Kill current pane | `Ctrl-b` x|

# Others

|Description|Command|
|:--|:--|
|Help | `Ctrl-b` ?|
|Display time | `Ctrl-b` t|
