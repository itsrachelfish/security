# security
Random files I've found while fixing hacked sites for friends

CC0 license because I don't really own this code. Does anybody really?

Searching for an absurd amount of indenting can be an easy way to spot backdoors.

```
grep -r "                                                                                                                                     " .
```

Or you can look through diffs to spot long lines, though you might end up sifting through legitimate minified code as well.
Or you can use this handy grep instead:

```
grep -rIE --exclude "*.js" --exclude "*.css" --exclude "*.svg" ".{500}" . 
```


### Pretty cool command, btw:

```
cp --parents
```
