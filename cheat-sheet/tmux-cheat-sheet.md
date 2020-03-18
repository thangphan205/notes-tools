# tmux Cheat Sheet
# 1. Session

|Command line                   | Description|
|-------------------------------|------------|
|$ tmux                         | open new session|
|$ tmux ls                      |list all sessions|
|$ tmux new -s <session_name>   | open new session with name is session_name|
|$ tmux a                       | attaced to last session|
|$ tmux a -t <session_name>     | attact to session with name session_name|
|$ tmux kill-session -a         | kill all sessions except current|
|Ctrl + b + d                   |detach from session|
|Ctrl + b + (                   | Move to previous session|
|Ctrl + b + )                   | Move to next session|