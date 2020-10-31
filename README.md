![image](https://user-images.githubusercontent.com/5031388/97772891-55511e80-1b08-11eb-958a-234dba5e6ff5.png)

This has a small change to tkmarsh's tronClock that makes it compatible with CLI screensavers, if you find yourself in that situation a la `tmux`, and adds colors.

Complile using:
`gcc nclock.c -lncurses`

To configure `tmux`, edit your configuration file (either `~/.tmux.conf` or at `/etc/tmux.conf`, whatever is available) with the following:
```
set -g lock-after-time 300 # or some abstract number in seconds, your call man
set -g lock-command /PATH/TO/YOUR/COMPILED/CLOCK/ENJOY
```

ncurses library is a pre-req for this repo.
