# PyQuery

## jquery like queries on command line shell

### usage

```
$ ./pyquery-cli -h
Usage:
-h, --help
-o, --output
-v, --version
-s, --select   'query'
-a, --attr     'attr_name'
-t, --text
-H, --html
-f, --file     <file>
```
### examples

testfile.html:
```
<html><input id="pippo" name="kkk" value="23" /></html>
```

```
$ ./pyquery-cli -f test/testfile.html -s'#pippo'
<input id="pippo" name="kkk" value="23"/>
```

```
$ ./pyquery-cli -f test/testfile.html -s'#pippo' -a 'name'
kkk
```
