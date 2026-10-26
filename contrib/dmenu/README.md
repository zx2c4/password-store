`passmenu` is a [dmenu][]-based interface to [pass][], the standard Unix
password manager. This design allows you to quickly copy a password to the
clipboard without having to open up a terminal window if you don't already have
one open. If `--type` is specified, the password is typed using [xdotool][]
instead of copied to the clipboard.

On wayland [wmenu][] is used to replace dmenu and [kwin-type][] for KDE or
[ydotool][] for others to replace xdotool. Note that the latter requires access
to the [uinput][] device, so you'll probably need to add an extra udev rule or
similar to give certain non-root users permission.

# Usage

    passmenu [--type] [dmenu arguments...]

[pass]: http://www.zx2c4.com/projects/password-store/
[dmenu]: http://tools.suckless.org/dmenu/
[wmenu]: https://codeberg.org/adnano/wmenu
[xdotool]: http://www.semicomplete.com/projects/xdotool/
[kwin-type]: https://git.zx2c4.com/kwin-type/about/
[ydotool]: https://github.com/ReimuNotMoe/ydotool
[uinput]: https://www.kernel.org/doc/html/latest/input/uinput.html
