

- Swift
- Double
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new instance initialized to the given value, if it can be represented without rounding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(exactly other: Double)
```

## Parameters 

`other`  

The value to use for the new instance.

## Discussion

If `other` can’t be represented as an instance of `Double` without rounding, the result of this initializer is `nil`. In particular, passing NaN as `other` always results in `nil`.

```
let x: Double = 21.25
let y = Double(exactly: x)
// y == Optional.some(21.25)

let z = Double(exactly: Double.nan)
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

init?(exactly: Float)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: Float16)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: Float80)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: NSNumber)

