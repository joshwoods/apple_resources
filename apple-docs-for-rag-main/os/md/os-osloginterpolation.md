

- os
-  OSLogInterpolation 

Structure

# OSLogInterpolation

A container for the elements of a log message.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
@frozen
struct OSLogInterpolation
```

## Overview

An OSLogInterpolation structure contains a formatted string and its interpolated arguments. Don’t create OSLogInterpolation structures directly. The system creates them automatically when you log messages using the Logger object.

When you craft log messages, you may incorporate content from your code’s variables directly into the message strings. When you do, the logging system creates OSLogInterpolation structures to store those values. The structure stores the provided values as-is, and the logging system formats those values as strings only in the final log message. To change the final appearance of a value, include additional parameters along with the value. Consider the following example, which logs values of several different types:

```
logger.log("\(taskID) \(giftCardID) \(serverID) \(seconds)")
```

For values that are variable in length, formatting them makes the log message easier to read. In the preceding example, `giftCardID` and `seconds` contain variable-length values. The following example fixes the formatting issues by making all gift card IDs the same width and aligning them to the left edge of the available space. The example also formats each seconds value as a fixed-point number with only two digits to the right of the decimal point.

```
logger.log("\(taskID) \(giftCardID, align: .left(columns: GiftCard.maxIDLength)) \(serverID) \(seconds, format: .fixed(precision: 2))")
```

Because strings and custom objects may contain user-sensitive information, the logging system redacts those values by default, however, it doesn’t redact numerical values. The resulting log message displays a string like `` instead of the actual value. If you know the value doesn’t include sensitive data, change the privacy setting using the `privacy` parameter, as the following example shows:

```
logger.log("Paid with bank account \(accountNumberString)")   // Redacted by default
logger.log("Ordered smoothie \(smoothieName, privacy: .public)")  // Visible!
```

## Topics

### Appending Strings

func appendInterpolation(@autoclosure () -> String, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated string.

func appendInterpolation(@autoclosure () -> String, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated string with the specified attributes.

### Appending Signed Integers

func appendInterpolation(@autoclosure () -> Int, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated integer.

func appendInterpolation(@autoclosure () -> Int8, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated 8-bit integer.

func appendInterpolation(@autoclosure () -> Int16, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated 16-bit integer.

func appendInterpolation(@autoclosure () -> Int32, format: OSLogInt32ExtendedFormat, privacy: OSLogPrivacy)

Appends an interpolated 32-bit integer.

func appendInterpolation(@autoclosure () -> Int32, format: OSLogInt32ExtendedFormat, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated 32-bit integer with the specified attributes.

func appendInterpolation(@autoclosure () -> Int32, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated 32-bit integer with the specified alignment.

func appendInterpolation(@autoclosure () -> Int64, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated 64-bit integer.

### Appending Unsigned Integers

func appendInterpolation(@autoclosure () -> UInt, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated unsigned integer.

func appendInterpolation(@autoclosure () -> UInt8, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated unsigned 8-bit integer.

func appendInterpolation(@autoclosure () -> UInt16, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated unsigned 16-bit integer.

func appendInterpolation(@autoclosure () -> UInt32, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated unsigned 32-bit integer.

func appendInterpolation(@autoclosure () -> UInt64, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated unsigned 64-bit integer.

### Appending Doubles

func appendInterpolation(@autoclosure () -> Double, format: OSLogFloatFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated double.

func appendInterpolation(@autoclosure () -> Double, format: OSLogFloatFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated double with the specified attributes.

### Appending Floats

func appendInterpolation(@autoclosure () -> Float, format: OSLogFloatFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated float.

func appendInterpolation(@autoclosure () -> Float, format: OSLogFloatFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated float with the specified attributes.

### Appending Boolean Values

func appendInterpolation(@autoclosure () -> Bool, format: OSLogBoolFormat, privacy: OSLogPrivacy)

Adds a Boolean argument to the message.

### Appending Generic Types

func appendInterpolation&lt;T>(@autoclosure () -> T, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated textual representation of a type.

func appendInterpolation&lt;T>(@autoclosure () -> T, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated textual representation of a type using the specified attributes.

func appendInterpolation&lt;T>(@autoclosure () -> T, format: OSLogIntegerFormatting, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated numeric type using the specified attributes.

func appendInterpolation(@autoclosure () -> any Any.Type, align: OSLogStringAlignment, privacy: OSLogPrivacy)

Appends an interpolated type description.

func appendInterpolation(@autoclosure () -> any Any.Type, align: OSLogStringAlignment, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated type description with the specified attributes.

### Appending Pointer Data

func appendInterpolation(@autoclosure () -> UnsafeRawPointer, bytes: @autoclosure () -> Int, format: OSLogPointerFormat, privacy: OSLogPrivacy)

Appends interpolated pointer data.

func appendInterpolation(@autoclosure () -> UnsafeRawPointer, bytes: @autoclosure () -> Int, format: OSLogPointerFormat, privacy: OSLogPrivacy, attributes: String)

Appends interpolated pointer data with the specified attributes.

func appendInterpolation(@autoclosure () -> UnsafeRawBufferPointer, format: OSLogPointerFormat, privacy: OSLogPrivacy)

Appends an interpolated collection of raw bytes.

func appendInterpolation(@autoclosure () -> UnsafeRawBufferPointer, format: OSLogPointerFormat, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated collection of raw bytes with the specified attributes.

### Appending Objects

func appendInterpolation(@autoclosure () -> NSObject, privacy: OSLogPrivacy)

Appends an interpolated object description.

func appendInterpolation(@autoclosure () -> NSObject, privacy: OSLogPrivacy, attributes: String)

Appends an interpolated object description with the specified attributes.

### Instance Methods

func appendInterpolation(@autoclosure () -> Int, format: OSLogIntExtendedFormat, privacy: OSLogPrivacy, attributes: String)

func appendInterpolation(@autoclosure () -> any Error, privacy: OSLogPrivacy, attributes: String)

func appendInterpolation(@autoclosure () -> (any Error)?, privacy: OSLogPrivacy, attributes: String)

func appendInterpolation(@autoclosure () -> NSObject?, privacy: OSLogPrivacy, attributes: String)

## Relationships

### Conforms To

- StringInterpolationProtocol

## See Also

### Value Interpolation

enum OSLogIntExtendedFormat

Options for expanding bit rate information stored as an int during logging.

