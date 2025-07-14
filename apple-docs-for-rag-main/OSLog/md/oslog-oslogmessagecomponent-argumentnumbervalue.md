

- OSLog
- OSLogMessageComponent
-  argumentNumberValue 

Instance Property

# argumentNumberValue

The argument formatted as a number.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var argumentNumberValue: NSNumber? { get }
```

## Discussion

The `argumentNumberValue` property can be `nil` if the argument can’t be decoded. For example, redacted arguments and the last component can’t be decoded.

## See Also

### Accessing the Argument

var argumentDataValue: Data?

The argument formatted as a sequence of bytes.

var argumentDoubleValue: Double

The argument formatted as a double.

var argumentInt64Value: Int64

The argument formatted as a signed 64-bit integer.

var argumentStringValue: String?

The argument formatted as a string.

var argumentUInt64Value: UInt64

The argument formatted as an unsigned 64-bit integer.

