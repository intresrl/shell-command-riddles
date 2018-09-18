Create a file into every empty folder
=====================================

As you probably know, git version control system does not keep track of empty folders.

If you want to commit a directory structure you must put a dummy file in each empty folder.
It is common to name such file `.gitkeep`

In this exercise you should write a script using basic unix commands that adds a `.gitkeep` file in every empty folder under current path.

You can create a sample structure with `mkdir -p a/b/c d/e f`: your script should add the new file in folders `c`, `e` and `f`

You can check the results with `ls -Ra` which lists recursively all files, including hidden ones (like `.gitkeep` since it begins with a `.`)
