

- Swift
- Double
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new instance from the given value, if it can be represented exactly.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(exactly value: Source) where Source : BinaryFloatingPoint
```

## Parameters 

`value`  

A floating-point value to be converted.

## Discussion

If the given floating-point value cannot be represented exactly, the result is `nil`.

## See Also

### Converting with No Loss of Precision

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

init?(exactly: Float80)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: NSNumber)

