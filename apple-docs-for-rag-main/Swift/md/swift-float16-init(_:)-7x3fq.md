

- Swift
- Float16
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance that approximates the given value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(_ other: Double)
```

## Parameters 

`other`  

The value to use for the new instance.

## Discussion

The value of `other` is rounded to a representable value, if necessary. A NaN passed as `other` results in another NaN, with a signaling NaN value converted to quiet NaN.

```
let x: Double = 21.25
let y = Float16(x)
// y == 21.25

let z = Float16(Double.nan)
// z.isNaN == true
```

