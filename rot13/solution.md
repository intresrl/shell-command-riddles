One possible approach is to use the `tr` command that translates a set of characters into another.

```echo cypher me | tr abcdefghijklmnopqrstuvwxyz nopqrstuvwxyzabcdefghijklm```

Also `sed` has the same ability with the `y` command

```echo cypher me | sed 'y/abcdefghijklmnopqrstuvwxyz/nopqrstuvwxyzabcdefghijklm/'```

Using the **Character Classes** is possible to avoid writing all the letters of the alphabet and it is also possible to manage easly the case of the character!

```bash
echo cypher ME | tr a-zA-Z n-za-mN-ZA-N
```
