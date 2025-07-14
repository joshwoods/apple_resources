

- AppKit
- NSCell
-  stringValue 

Instance Property

# stringValue

The cell’s value as a string.

macOS

``` source
@MainActor
var stringValue: String { get set }
```

## Discussion

This property uses the objectValue property to access the actual value. If no formatter is assigned to the cell or if the formatter cannot “translate” a new string appropriately, the cell is flagged as having an invalid object. If the cell’s object is not an NSString object or cannot be converted to one, this property contains an empty string. If the cell is not a text-type cell, this method converts it to one before setting the object value.

If you use a class that has an attributedStringValue property, the cell gets the string from that property instead of this one.

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

var doubleValue: Double

The cell’s value as a double-precision floating-point number.

var floatValue: Float

The cell’s value as a single-precision floating-point number.

