## Ncmpcpppppppppppppp

![tmux session with ncmpcpp and cover](../.pictures/music.png)

## Dependencies

+ inotify-tools
+ ueberzug (python package)
+ ncmpcpp
+ tmux

## Installation

Under `$HOME/.config/ncmpcpp/tmux_config`, add this line to run the script to generate cover picture

```config
execute_on_song_change = "$HOME/.config/ncmpcpp/ncmpcpp-ueberzug/ncmpcpp_cover_art.sh"
```

Please note that both script `art.sh` and `cover.sh` needs to be copied over to your `~/.ncmpcpp` folder

### art.sh

The script is inspired by http://dotshare.it/dots/1533/
This script is much simpler as `ffmpeg` can extract cover art and resize it in one line ;)


### cover.sh

Display the cover picture (`/tmp/cover.png`) directly in the terminal.

Thanks to [/seebye/ueberzug](https://github.com/seebye/ueberzug) for the amazing library (it works perfectly in sxt and tmux).
Install this python dependency:

```shell
$ sudo pip3 install ueberzug
```

## Run

`$HOME/.config/ncmpcpp/tmux_session` is a tmux session file that will open the `cover.sh` script and `ncmpcpp` as in the above picture.

Add this alias in your `{~/.config/fish/config.fish,~/.zshrc,~/.bash}` file

```shell
alias ncmpcpp-tmux='tmux new-session -s $fish_pid "tmux source-file $HOME/.config/ncmpcpp/tsession"' # Tmux session with ncmpcpp and cover art
```

Run `ncmpcpp-tmux` to see the music ;)
