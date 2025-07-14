

- Foundation
- NSString
-  boolValue 

Instance Property

# boolValue

The Boolean value of the string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var boolValue: Bool { get }
```

## Discussion

This property is true on encountering one of “Y”, “y”, “T”, “t”, or a digit 1-9—the method ignores any trailing characters. This property is false if the receiver doesn’t begin with a valid decimal text representation of a number.

The property assumes a decimal representation and skips whitespace at the beginning of the string. It also skips initial whitespace characters, or optional -/+ sign followed by zeroes.

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

var longLongValue: Int64

The `long long` value of the string.

