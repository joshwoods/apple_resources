

- OSLog
- OSLogMessageComponent
-  argumentStringValue 

Instance Property

# argumentStringValue

The argument formatted as a string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var argumentStringValue: String? { get }
```

## Discussion

The `argumentStringValue` property can be `nil` if the argument can’t be decoded. For example, redacted arguments or the last component can’t be decoded.

## See Also

### Accessing the Argument

var argumentDataValue: Data?

The argument formatted as a sequence of bytes.

var argumentDoubleValue: Double

The argument formatted as a double.

var argumentInt64Value: Int64

The argument formatted as a signed 64-bit integer.

var argumentNumberValue: NSNumber?

The argument formatted as a number.

var argumentUInt64Value: UInt64

The argument formatted as an unsigned 64-bit integer.

