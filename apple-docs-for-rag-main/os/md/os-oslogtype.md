

- os
-  OSLogType 

Structure

# OSLogType

The various log levels that the unified logging system provides.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct OSLogType
```

## Overview

A log level controls how and when the system writes a message to the unified logging system. To write a message with a specific log level, create a Logger and call its log(level:_:) method. Alternatively, call the method that corresponds to the desired log level, such as debug(_:) or fault(_:).

## Topics

### Getting Log Types

static let debug: OSLogType

The debug log level.

static let info: OSLogType

The informative log level.

static let `default`: OSLogType

The default log level.

static let error: OSLogType

The error log level.

static let fault: OSLogType

The fault log level.

### Creating a Log Type

init(UInt8)

Creates a log type from the specified value.

init(rawValue: UInt8)

Creates a log type from the specified raw value.

### Getting the Raw Value

var rawValue: UInt8

The log type’s raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Log Messages

struct Logger

An object for writing interpolated string messages to the unified logging system.

Message Argument Formatters

Manage the privacy and presentation of the message’s interpolated values using type-aware formatters.

