# tmux
`^B` means `Ctrl+B`
## sessions
- create a new session `tmux new -s sess_name`
- attach to an existing session `tmux attach -t sess_name`
- switch to an existing session `tmux switch -t sess_name`
- list existing session `tmux ls`


sortcuts  cheat   
- `^B n` -> next window = 
- `^B [0-9]` -> select window by number `^B :select-window -t [0-9]`
- `^B c` -> create new window
- `^B ,` -> rename window
- `^B "` -> split window vertically in two panes
- `^B %` -> split window horiz
- `^B { or }` -> swap panes
- `^B q [1,2,3,..]` -> select pane by number
- `^B [Up, Down, Left, Right]` -> switch panes
