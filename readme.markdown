some goals from mind

- replacement for {ba,z,}sh:
    - no to compatibility, yes to comfort
- go routines


variable declarations:
```
a = 1
f = 3.14
b = "2"
c = [1, "2", [3]]
d = {"a": 1, "b": "2", "xxx": [1, 2]}
e = true
```

a - int64
f - float64
b - string
c - []interface{}
d - map[string]interface{}
e - bool


no more var hell


no more func/fn/function/func!/def/define hell

function declaration must have a input variables signature
no more bash `local name=` hell
```
database:connect(host, user, pass) {
    // body
}
```


variable expansion
no more bash-like bracket bullshit magic, replace ${var:-no} ${var:+yes} and
other features on builtins


send `[[ ]]` brackets to the trash, if-statements must be written using
following syntax:
```
if b > a {
    // positive body
} else if b < a {
    // whatever body
} else {
    // negative body
}
```

if/else statements can't be written without `{}`, code must be obvious.

builtins
copy(source, destination)
append(slice, element)
delete(map, key)
len(slice)
print(args)
printf(format, args)
is(var, type)
in(slice, var)
in(map, var)
keys(map)
