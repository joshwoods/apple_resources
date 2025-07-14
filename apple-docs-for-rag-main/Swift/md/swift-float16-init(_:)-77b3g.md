

- Swift
- Float16
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance initialized to the given value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(_ other: Float16)
```

## Parameters 

`other`  

The value to use for the new instance.

## Discussion

The value of `other` is represented exactly by the new instance. A NaN passed as `other` results in another NaN, with a signaling NaN value converted to quiet NaN.

```
let x: Float16 = 21.25
let y = Float16(x)
// y == 21.25

let z = Float16(Float16.nan)
// z.isNaN == true
```

