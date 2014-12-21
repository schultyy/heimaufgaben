---
title: Directory contents
---

# Directory contents

## Description

Write a command line program which gets a directory path as argument and writes all directories and files into a file.

```bash
$ ruby list_directory.rb /Users/jan/temp
> Reading...
> Writing results to contents.txt
$ cat contents.txt
[f] cat1.png
[f] cat2.png
[f] cat3.png
[d] more_cats
  [f] meow.png
  [f] the_cat_from_the_internet.png
[f] hello.txt
[d] foo
  [d] bar
    [f] baz.txt
```

A file is prefixed by `[f]`, a directory with a `[d]`. If a directory contains subdirectories, those should also appear including their subdirectories and files.
