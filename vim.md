# Vim cheatsheet

## Search and replace

### [substitute](https://vim.fandom.com/wiki/Search_and_replace)

Find each occurrence of *foo* in the current line, and replace it with *bar*.

``` vim
:s/foo/bar/g
```

Find each occurrence of *foo* in whole file, and replace it with *bar*.

``` vim
:%s/foo/bar/g
```

### [grep](https://vim.fandom.com/wiki/Power_of_g)

This acts on the specified *range* __default whole file__, by executing the *command* for each line matching pattern.

``` vim
:[range]g/pattern/command
```

Delete all lines matching a *pattern*.

``` vim
:g/pattern/d
```

Delete all lines that do __not__ match a *pattern*.

``` vim
:g!/pattern/d
:v/pattern/d
```

## retab

Replace all sequences of white-space containing a *Tab* with new strings of white-space using the new tabstop value given. If you do not specify a new tabstop size or it is zero, Vim uses the current value of 'tabstop'.

``` vim
:[range]retab[!] [new_tabstop]
```

