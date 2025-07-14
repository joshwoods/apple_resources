

- AppKit
- NSCell
-  objectValue 

Instance Property

# objectValue

The cell’s value as an Objective-C object.

macOS

``` source
@MainActor
var objectValue: Any? { get set }
```

## Discussion

To be valid object value, the cell must have a formatter capable of converting the object to and from its textual representation. The value of this property is `nil` if an object has not been assigned to the cell.

## See Also

### Managing Cell Values

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

var floatValue: Float

The cell’s value as a single-precision floating-point number.

