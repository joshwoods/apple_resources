

- Swift
- Double
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new instance initialized to the given value, if it can be represented without rounding.

macOS 10.10+

``` source
init?(exactly other: Float80)
```

## Parameters 

`other`  

The value to use for the new instance.

## Discussion

If `other` can’t be represented as an instance of `Double` without rounding, the result of this initializer is `nil`. In particular, passing NaN as `other` always results in `nil`.

```
let x: Float80 = 21.25
let y = Double(exactly: x)
// y == Optional.some(21.25)

let z = Double(exactly: Float80.nan)
// z == nil
```

## See Also

### Converting with No Loss of Precision

init?&lt;Source>(exactly: Source)

Creates a new instance from the given value, if it can be represented exactly.

init?&lt;Source>(exactly: Source)

Creates a new value, if the given integer can be represented exactly.

init?&lt;Source>(exactly: Source)

Creates a new value, if the given integer can be represented exactly.

init?(exactly: Double)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: Float)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: Float16)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: NSNumber)

