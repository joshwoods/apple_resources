

- AppKit
- NSCell
-  hasValidObjectValue 

Instance Property

# hasValidObjectValue

A Boolean value that indicates whether the cell has a valid object value.

macOS

``` source
@MainActor
var hasValidObjectValue: Bool { get }
```

## Discussion

The value of this property is true if the cell has a valid object value or false if it does not. A valid object value is one that the cell’s formatter can “understand.” Objects are always assumed to be valid unless they are rejected by the formatter. Invalid objects can still be accepted by the delegate of the cell’s NSControl object (using the control(_:didFailToFormatString:errorDescription:) delegate method).

## See Also

### Managing Cell Values

var objectValue: Any?

The cell’s value as an Objective-C object.

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

