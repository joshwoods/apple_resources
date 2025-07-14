

- Swift
- Float16
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new value, if the given integer can be represented exactly.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(exactly value: Source) where Source : BinaryInteger
```

Available when `RawSignificand` conforms to `FixedWidthInteger`.

## Parameters 

`value`  

The integer to convert to a floating-point value.

## Discussion

If the given integer cannot be represented exactly, the result is `nil`.

