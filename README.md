# lf-config

This is the repository containing the lf configuration file.

lf (as in "list files") is a terminal file manager written in Go with a heavy inspiration from ranger file manager [[repository](https://github.com/gokcehan/lf), [documentation](https://pkg.go.dev/github.com/gokcehan/lf)].

Usage environment: macOS 13.6.1 Ventura and zsh via [warp](https://www.warp.dev/) terminal with Light theme.


## Keybindings

| Command | Keybinding |
|---------| :------------: |
| shell | $ or enter |
| shell-pipe | % |
| shell-wait | !  |
| shell-async | &  |
| quit | q |
| up | ↑ |
| down | ↓ |
| page-up | u |
| page-down | d |
| top | U |
| bottom | D |
| updir | ← |
| open | → |
| delete | delete |
| toggle | space |
| glob-select | ts |
| glob-unselect | tu |
| invert | ti |
| invert-below | tb |
| copy | c |
| cut | C |
| paste | p |
| clear | l |
| redraw | rd |
| reload | rl |
| mark-save | ms |
| mark-load | ml |
| mark-remove | mr |
| show-results | ` |
| execute-file | x |
| execute-file | X |
| make-directory | ctrl-d|
| create-file | ctrl-f |
| rename-file | ctrl-r |
| create-tar-archive | at |
| create-zip-archive | az |
| extract-archive | ae |
| copy-current-dir-to-clipboard | alt-d |
| copy-full-file-name-to-clipboard | alt-f |
| open-in-finder | alt-o |
| show-hidden | zh |
| reverse-sort-direction | zr |
| hide-info | zn |
| show-info-size | zs |
| show-info-time | zt |
| show-info-size:time | za |
| show-info-dirsize | zd |
| sortby-natural | sn |
| sortby-size | ss |
| sortby-time | st |
| sortby-atime | sa |
| sortby-ctime | sc |
| sortby-ext | se |
| go-home-dir | gh |
| go-downloads-dir | gd |
| go-projects-dir | gp |
| go-root-dir | gr |
| go-dir | G |
| find | f |
| find-back | F |
| find-next | ] |
| find-prev | [ |
| search | / |
| search-back | ? |
| search-next | n |
| search-prev | N |


## Colors

Based on the [documentation](https://github.com/gokcehan/lf/blob/master/doc.md#colors), LF_COLORS has the same syntax as LS_COLORS. LS_COLOR syntax consists of four parts:

```
KEY   EFFECT;COLOR;BACKGROUND_COLOR
```  
  
### KEY

| Code | Description | Notes |
| :---: |--|---|
| no | NORMAL, NORM | Global default
| fi | FILE | Normal file |
| di | DIR | Directory |
| ln | SYMLINK, LINK, LNK | Symbolic link |
| pi | FIFO, PIPE | Named pipe |
| do | DOOR | Door |
| bd | BLOCK, BLK | Block device |
| cd | CHAR, CHR | Character device |
| or | ORPHAN | Symbolic link pointing to a non-existent file |
| so | SOCK | Socket |
| su | SETUID | File that is setuid (u+s) |
| sg | SETGID | File that is setgid (g+s) |
| tw | STICKY_OTHER_WRITABLE | Directory that is sticky and other-writable (+t,o+w) |
| ow | OTHER_WRITABLE | Directory that is other-writable (o+w) and not sticky |
| st | STICKY | Directory with the sticky bit set (+t) and not other-writable |
| ex | EXEC | Executable file (i.e. has 'x' set in permissions) |
| mi | MISSING | Non-existent or missing file pointed to by a symbolic link (visible when you type ls -l) |
| lc | LEFTCODE, LEFT | Opening terminal code |
| rc | RIGHTCODE, RIGHT | Closing terminal code |
| ec | ENDCODE, END | Non-filename text |
| ca | CAPABILITY | File with capability |
| mh | MULTIHARDLINK | Hard link |
| rs | RESET | Reset to no color |
| *.ext | FILE TYPE CODE | Any file with any extension |


### EFFECT

| Code | Property |
| :---: |--|
| 00 | Default color |
| 01 | Bold font |
| 04 | Underlined |
| 05 | Flashing text |
| 07 | Reverse |
| 08 | Concealed |


### COLOR

| Code | Property |
| :---: |---|
| 30 | Black |
| 31 | Red |
| 32 | Green |
| 33 | Orange |
| 34 | Blue |
| 35 | Purple |
| 36 | Cyan |
| 37 | Grey |


### BACKGROUND COLOR

| Code | Property |
| :---: |---|
| 40 | Black background |
| 41 | Red background |
| 42 | Green background |
| 43 | Orange background |
| 44 | Blue background |
| 45 | Purple background |
| 46 | Cyan background |
| 47 | Grey background |


### ADDITIONAL COLOR

| Code | Property |
| :---: |---|
| 90 | Dark grey |
| 91 | Light red |
| 92 | Light green |
| 93 | Yellow |
| 94 | Light blue |
| 95 | Light purple |
| 96 | Turquoise |
| 97 | White |
|——|
| 100 | Dark grey background |
| 101 | Light red background |
| 102 | Light green background |
| 103 | Yellow background |
| 104 | Light blue background |
| 105 | Light purple background |
| 106 | Turquoise background |
| 107 | White background |

### Default Colors

```
ln  01;36
or  31;01
tw  01;34
ow  01;34
st  01;34
di  01;34
pi  33
so  01;35
bd  33;01
cd  33;01
su  01;32
sg  01;32
ex  01;32
fi  00
```
