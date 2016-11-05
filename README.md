# git-intro-noname
Git-Intro-NoName

- clone this repo
- Install vim-plug: [vim-plug](https://github.com/junegunn/vim-plug#installation)

Start with given vimrc:
vim -u .vimrc

## Notes

### Moving with cursor
h j k l => moving with cursor

0 => beginning of line

$ => end of line

w => Move word 

W => Move WORD ( separated by space )

b => backwards wordswise

B => backwards WORD-wise

e => Move to end of word

E => Move to end of word

f F find next character

t T till next character

/ ? search

repeat: 3w 

G => end of file

gg => beginnign of file

ctr-d => scroll down

ctr-u => scroll up

ctr-e / ctrl-y => scroll up/down linewise


### Action

d => delete

v => mark characterwise

V => mark linewise

y => copy

p => paste before

P => paste after


### Normalmode -> Insertmode

i => insert before cursor

a => append after cursor

I => insert at beginning 

A => Append at the end of line

o => before current line

O => after current line

J => join 

### Editing
c => change

C => Change till end of line

d => delete

D => Delete till end of line

S => change line

caw => change a word

ciw => change within word

ciw => change within word

cf. => change until .

### Edit code

ci( 

ca(

ciB

ci{

cit


### Normal mode

:s/search/replace        => one line

:%s/search/replace       => while file

:s/<ctrl-r><ctrl-w>/bla/ => word under cursor

:copy

:move

:g/bla/d

:v/bla/d

:g/bla/move$

:ol => old files

:changes 

:jump

ctrl-o => jump to last visited files

gi => insert mode at last inserte

qq -> macro

CTRL-V => block mode

:w => write

:q! quit

## With terminal

=> mark => execute external command and return result

:'<, '>!cut -f 1 -d' '

:'<, '>!grep -i 'bla'

:!ls

:r !ls -lah

ls -lah |  vim -


