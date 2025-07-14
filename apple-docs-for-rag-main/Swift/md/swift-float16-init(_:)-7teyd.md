

- Swift
- Float16
-  init(\_:) 

Initializer

# init(\_:)

Creates a new value, rounded to the closest possible representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ value: Source) where Source : BinaryInteger
```

Available when `RawSignificand` conforms to `FixedWidthInteger`.

## Parameters 

`value`  

The integer to convert to a floating-point value.

## Discussion

If two representable values are equally close, the result is the value with more trailing zeros in its significand bit pattern.

