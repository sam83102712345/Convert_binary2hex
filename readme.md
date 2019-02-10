# Convert binary string to hex string

Ex: 
You have a list [0000, 0000, 0000, 0100, 1000, 1101] and you want to get 00048D

1. Concatenate all string
```
>>> a = ['0000', '0000', '0000', '0100', '1000', '1101']
>>> b = ''.join(a)
>>> b
'000000000000010010001101'
```

2. Use function "format" to convert

```
>>> "{:0>6X}".format(int(''.join(b), 2))
'00048D'
```

P.S "{:0> **6** X}".format(int(''.join(b), 2)), the number '6' means that how many numbers you want to represent. 
