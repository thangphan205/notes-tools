# tmux Cheat Sheet
Shortcut example: 

Ctrl+b [d] => Press [Ctrl], [b] button at the same time, then realse [Ctrl] and [b] button, then press [d] button.

Ctrl + b + d => Press [Ctrl], [b], [d] button at the same time.
## 1. Session

|Command line                   | Description|
|-------------------------------|------------|
|$ tmux                         | open new session|
|$ tmux ls                      |list all sessions|
|$ tmux new -s <session_name>   | open new session with name is session_name|
|$ tmux a                       | attaced to last session|
|$ tmux a -t <session_name>     | attact to session with name session_name|
|$ tmux kill-session -a         | kill all sessions except current|
|Ctrl+b  [d]                   |detach from session|
|Ctrl+b  [(]                   | Move to previous session|
|Ctrl+b  [)]                   | Move to next session|

## 2. Shortcut Pane, Windows

|Shortcut           |Description        |
|-------------------|-------------------|
|Ctrl+b  [;]       |Toggle last active pane|
|Ctrl+b  [%]       |Split pane vertically|
|Ctrl+b  ["]       |Split pane horizontally|
|Ctrl+b  [{]       |Move current pane to left|
|Ctrl+b  [}]       |Move current pane to right|
|Ctrl+b  up/down/left/right arrow key| Move to pane up/down/left/right|
|Ctrl+b + up/down/left/right arrow key| Resize pane (press arrow key fast)|
|*Ctrl+d*           |*Close current pane*|
