

- AppKit
- NSCell
-  integerValue 

Instance Property

# integerValue

The cell’s value as an NSInteger type.

macOS 10.5+

``` source
@MainActor
var integerValue: Int { get set }
```

## Discussion

This property uses the objectValue property to access the actual value. If the cell is not a text-type cell or its contents are not scannable, the value in this property is `0`.

## See Also

### Managing Cell Values

var objectValue: Any?

The cell’s value as an Objective-C object.

var hasValidObjectValue: Bool

A Boolean value that indicates whether the cell has a valid object value.

var intValue: Int32

The cell’s value as an integer.

var stringValue: String

The cell’s value as a string.

var doubleValue: Double

The cell’s value as a double-precision floating-point number.

var floatValue: Float

The cell’s value as a single-precision floating-point number.

