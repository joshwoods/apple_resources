

- Swift
- Float80
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new instance from the given value, if it can be represented exactly.

macOS 10.10+

``` source
init?(exactly value: Source) where Source : BinaryFloatingPoint
```

## Parameters 

`value`  

A floating-point value to be converted.

## Discussion

If the given floating-point value cannot be represented exactly, the result is `nil`.

