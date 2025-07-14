

- Swift
- Float80
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance from the given value, rounded to the closest possible representation.

macOS 10.10+

``` source
init(_ value: Source) where Source : BinaryFloatingPoint
```

## Parameters 

`value`  

A floating-point value to be converted.

## Discussion

If two representable values are equally close, the result is the value with more trailing zeros in its significand bit pattern.

