

- Swift
- Double
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new instance initialized to the given value, if it can be represented without rounding.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init?(exactly other: Float16)
```

## Parameters 

`other`  

The value to use for the new instance.

## Discussion

If `other` can’t be represented as an instance of `Double` without rounding, the result of this initializer is `nil`. In particular, passing NaN as `other` always results in `nil`.

```
let x: Float16 = 21.25
let y = Double(exactly: x)
// y == Optional.some(21.25)

let z = Double(exactly: Float16.nan)
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

init?(exactly: Float80)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: NSNumber)

