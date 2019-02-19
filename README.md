Transfer files through the tmux scrollback buffer
to setup the scrollback buffer size, add the following to ~/.tmux.conf
`set-option -g history-limit 104857600`

To transfer files between machines:
1) on localhost start tmux
2) in tmux ssh to remote host
3) copy tmux-file-transfer using copy/paste
4) run ./tmux-file-transfer --send file_or_dir_to_send
5) on another terminal on localhost: run ./tmux-file-transfer --receive tmux_transfer.tar.gz
