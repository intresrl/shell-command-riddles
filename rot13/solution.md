One possible approach is to use the `tr` command that translates a set of characters into another.

```echo cypher me | tr abcdefghijklmnopqrstuvwxyz nopqrstuvwxyzabcdefghijklm```

Also `sed` has the same ability with the `y` command

```echo cypher me | sed 'y/abcdefghijklmnopqrstuvwxyz/nopqrstuvwxyzabcdefghijklm/'```
