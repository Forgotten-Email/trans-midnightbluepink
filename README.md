# ForgottenEmail's Dotfiles (WIP)

![Screenshot_2022-01-30-10-49-26_1360x768](https://user-images.githubusercontent.com/96489361/151721389-881c5068-be1d-40f9-b18c-54b53264b55a.png)

![Screenshot_2022-01-30-10-51-06_1360x768](https://user-images.githubusercontent.com/96489361/151721378-1ae65e37-9ab2-45a8-ac6b-1accfe207bf7.png)

![Screenshot_2022-01-30-10-45-16_1360x768](https://user-images.githubusercontent.com/96489361/151721406-b6d1d257-34db-4da2-a29f-6642f196e0dd.png)

![Screenshot_2022-01-30-10-52-19_1360x768](https://user-images.githubusercontent.com/96489361/151721376-91c127be-1fbd-4e70-9368-067ea57ca723.png)

## Notes
- If polybar is too small change `height` in `.config/polybar/config.ini` to a suitable:
```
; Dimension defined as pixel value (e.g. 35) or percentage (e.g. 50%),
; the percentage can optionally be extended with a pixel offset like so:
; 50%:-10, this will result in a width or height of 50% minus 10 pixels
width = 100%
height = 25
```
- To disable Conkeww comment out these lines in `~/.config/bspwm/bspwmrc`:
```
# Launch Conkeww
#sed -i "s/colors\/color-.*/colors\/color-one-dark.yuck\")/g" $HOME/.config/conkeww/eww.yuck
#eww --config $HOME/.config/conkeww/ open conkeww-main
```
## To Do
- Add a list of dependencies
- Update screenshots
- Make an install script
- Remove references to old directories in the polybar module files
- Make independent of Axyl OS
