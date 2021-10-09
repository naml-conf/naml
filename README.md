# naml
the naml spec

## what is naml?
naml (naomi's altered markup language) is an attempt to create a config format which is readable and easy to edit, while being less horrible to parse than YAML, and not as confusing to look at as JSON.

### basic syntax

you define a block like you would in a curlybraced language:

```
block {

}
```

to just have a value, do it like the following

```
key = value
```
every line can only have one key and value or block opening/closing

```
stringExample = "string text" 
block {
  double = 0.01
  nestedBlock {
    nestedInteger = 10581
    nestedBoolean = y
  }
}
```
as seen above, a string value has to be enclosed in double quotes -> `string = "yeetus"`. floating point numbers are easily defined with a decimal point -> `double = 0.0001`. integers are the same, but without the decimal point. a boolean value is defined with either y or n.
