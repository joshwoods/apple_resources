

- os
- Logging
-  Message Argument Formatters 

API Collection

# Message Argument Formatters

Manage the privacy and presentation of the message’s interpolated values using type-aware formatters.

## Topics

### Privacy Options

struct OSLogPrivacy

The privacy options that determine when to redact or display values in log messages.

### Value Formatters

enum OSLogBoolFormat

The formatting options for Boolean values.

struct OSLogIntegerFormatting

The formatting options for integer values.

enum OSLogInt32ExtendedFormat

The formatting options for 32-bit integer values.

struct OSLogFloatFormatting

The formatting options for double and floating-point numbers.

enum OSLogPointerFormat

The formatting options for pointer data.

### Value Interpolation

struct OSLogInterpolation

A container for the elements of a log message.

enum OSLogIntExtendedFormat

Options for expanding bit rate information stored as an int during logging.

### String Alignment

struct OSLogStringAlignment

The alignment options for interpolated strings.

## See Also

### Log Messages

struct Logger

An object for writing interpolated string messages to the unified logging system.

struct OSLogType

The various log levels that the unified logging system provides.

