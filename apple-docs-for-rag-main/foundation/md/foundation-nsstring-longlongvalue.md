

- Foundation
- NSString
-  longLongValue 

Instance Property

# longLongValue

The `long long` value of the string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var longLongValue: Int64 { get }
```

## Discussion

The `long long` value of the string, assuming a decimal representation and skipping whitespace at the beginning of the string. This property is `LLONG_MAX` or `LLONG_MIN` on overflow. This property is `0` if the receiver doesn’t begin with a valid decimal text representation of a number.

This property uses formatting information stored in the non-localized value; use an Scanner object for localized scanning of numeric values from a string.

## See Also

### Related Documentation

func scanInt32(UnsafeMutablePointer&lt;Int32>?) -> Bool

Scans for an int value from a decimal representation, returning a found value by reference.

Deprecated

### Getting Numeric Values

var doubleValue: Double

The floating-point value of the string as a `double`.

var floatValue: Float

The floating-point value of the string as a `float`.

var intValue: Int32

The integer value of the string.

var integerValue: Int

The `NSInteger` value of the string.

var boolValue: Bool

The Boolean value of the string.

