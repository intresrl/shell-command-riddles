With `find` you can also execute commands on results

To solve our exercise we issue a single find command that looks for empty (`-empty`) folders (`-type d`) and executes a touch command to create the gitkeep file in them.

`-exec` option has a couple of different syntaxes; in this case we used `-exec command {} \;` which calls the given command once for each path in the results, replacing `{}` with that path.

```bash
find . -type d -empty -exec touch {}/.gitkeep \;
```
