

- Swift
- Float80
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance initialized to the given value.

macOS 10.10+

``` source
init(_ other: Float80)
```

## Parameters 

`other`  

The value to use for the new instance.

## Discussion

The value of `other` is represented exactly by the new instance. A NaN passed as `other` results in another NaN, with a signaling NaN value converted to quiet NaN.

```
let x: Float80 = 21.25
let y = Float80(x)
// y == 21.25

let z = Float80(Float80.nan)
// z.isNaN == true
```

