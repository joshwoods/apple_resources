

- AppKit
- NSCell
-  floatValue 

Instance Property

# floatValue

The cell’s value as a single-precision floating-point number.

macOS

``` source
@MainActor
var floatValue: Float { get set }
```

## Discussion

This property uses the objectValue property to access the actual value. If the cell is not a text-type cell or the cell’s value is not scannable, this property contains the value `0`.

## See Also

### Managing Cell Values

var objectValue: Any?

The cell’s value as an Objective-C object.

var hasValidObjectValue: Bool

A Boolean value that indicates whether the cell has a valid object value.

var intValue: Int32

The cell’s value as an integer.

var integerValue: Int

The cell’s value as an NSInteger type.

var stringValue: String

The cell’s value as a string.

var doubleValue: Double

The cell’s value as a double-precision floating-point number.

