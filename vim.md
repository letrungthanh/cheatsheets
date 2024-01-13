# Vim cheatsheet

## retab

Replace all sequences of white-space containing a Tab with new strings of white-space using the new tabstop value given. If you do not specify a new tabstop size or it is zero, Vim uses the current value of 'tabstop'.

``` vim
:[range]retab[!] [new_tabstop]
```

