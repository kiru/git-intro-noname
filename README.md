# VIM introduction

VIM by default is configured badly. This repo provides a better config based on the [vim-sensible](https://github.com/tpope/vim-sensible)

In order to start the new configuration:

- clone this repo
- Install vim-plug: [vim-plug](https://github.com/junegunn/vim-plug#installation)
- Start vim with:
> vim -u .vimrc

Alternative: 
> cp <this-repo>/.vimrc ~/.vimrc
> vim

## Notes

### Motion
`h j k l` Navigation

`0` Jump to the beginning of the line
  
`$` End of line

`w` Word by word

`W` Word by w ( separated by space )

`b` Backwards word-by-word (reverse of `w` )

`B` Backwards word-by-word (Space separated)

`f K` Move to next character `K`
  
`/me` Serach for next occurence of me
  
`3{motion}` repeat motion 3 times
  
  
### More motions  
  
`e` Move to end of word
  
`E` Move to end of word (space separated)

`t T` Same as `f T` but cursor stops before T

`G` End of the file
  
`gg` Beginnign of file

`ctrl-d` scroll down

`ctr-u`scroll up

`ctr-e / ctrl-y` scroll up/down linewise

### Command

`d`delete

`c` change
  
`v` mark characterwise

`y` copy / yank
  
  
  
### More commands  
`V` mark linewise

`p` paste before

`P` paste after


### Normalmode -> Insertmode

`i` insert before cursor

`a` append after cursor

`I` insert at the beginning

`A` Append at the end of line

`o` before current line

`O` after current line

### Editing

`C` <=> `c$`
  
`D` <=> `d$`

`S` <=> `0C`

`caw` => change a word
  
`ciw` => change within word

`ciw` => change within word

`cf.` => change until .

### Edit code

`ci(`

`ca(`

`ciB`

`ci{`

`cit`

### Normal mode

:s/search/replace        => one line

:%s/search/replace       => whole file

:copy

:move

:g/bla/d

:v/bla/d

:g/bla/move$

  
#### Advaned commands
:ol => old files

:changes 

:jump

`ctrl-o` jump to last visited files

`gi` insert mode at last inserte

`qq` macro

`CTRL-V` block mode

`:w?`write

`:q!` quite

## With terminal

=> mark => execute external command and return result

`:'<, '>!cut -f 1 -d' '`

`:'<, '>!grep -i 'bla'`

`:!ls`

`:r !ls -lah`

`ls -lah |  vim -`
