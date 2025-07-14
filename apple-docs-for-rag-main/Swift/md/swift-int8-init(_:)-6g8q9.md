

- Swift
- Int8
-  init(\_:) 

Initializer

# init(\_:)

Creates an integer from the given floating-point value, rounding toward zero.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ source: Float)
```

## Parameters 

`source`  

A floating-point value to convert to an integer. `source` must be representable in this type after rounding toward zero.

## Discussion

Any fractional part of the value passed as `source` is removed, rounding the value toward zero.

```
let x = Int(21.5)
// x == 21
let y = Int(-21.5)
// y == -21
```

If `source` is outside the bounds of this type after rounding toward zero, a runtime error may occur.

```
let z = UInt(-21.5)
// Error: ...the result would be less than UInt.min
```

