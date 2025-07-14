

- Foundation
- NSString
-  doubleValue 

Instance Property

# doubleValue

The floating-point value of the string as a `double`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var doubleValue: Double { get }
```

## Discussion

This property doesn’t include any whitespace at the beginning of the string. This property is `HUGE_VAL` or `–HUGE_VAL` on overflow, `0.0` on underflow. This property is `0.0` if the string doesn’t begin with a valid text representation of a floating-point number.

This property uses formatting information stored in the non-localized value; use an Scanner object for localized scanning of numeric values from a string.

## See Also

### Related Documentation

func scanDouble(UnsafeMutablePointer&lt;Double>?) -> Bool

Scans for a double value, returning a found value by reference.

Deprecated

### Getting Numeric Values

var floatValue: Float

The floating-point value of the string as a `float`.

var intValue: Int32

The integer value of the string.

var integerValue: Int

The `NSInteger` value of the string.

var longLongValue: Int64

The `long long` value of the string.

var boolValue: Bool

The Boolean value of the string.

