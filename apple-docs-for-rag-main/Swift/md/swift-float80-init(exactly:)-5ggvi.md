

- Swift
- Float80
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new value, if the given integer can be represented exactly.

macOS 10.10+

``` source
init?(exactly value: Source) where Source : BinaryInteger
```

Available when `RawSignificand` conforms to `FixedWidthInteger`.

## Parameters 

`value`  

The integer to convert to a floating-point value.

## Discussion

If the given integer cannot be represented exactly, the result is `nil`.

