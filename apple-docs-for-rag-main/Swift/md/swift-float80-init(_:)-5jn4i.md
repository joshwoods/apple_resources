

- Swift
- Float80
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance that approximates the given value.

macOS 10.10+

``` source
init(_ other: Float)
```

## Parameters 

`other`  

The value to use for the new instance.

## Discussion

The value of `other` is rounded to a representable value, if necessary. A NaN passed as `other` results in another NaN, with a signaling NaN value converted to quiet NaN.

```
let x: Float = 21.25
let y = Float80(x)
// y == 21.25

let z = Float80(Float.nan)
// z.isNaN == true
```

