

- os
-  OSLogMessage 

Structure

# OSLogMessage

An object that represents a log message.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
@frozen
struct OSLogMessage
```

## Overview

Important

You don’t create instances of OSLogMessage directly. Instead, the system creates them for you when writing messages to the unified logging system using a Logger.

## Topics

### Getting the Message Details

var bufferSize: Int

The byte size of the buffer that the logging system receives.

let interpolation: OSLogInterpolation

The log message’s string interpolation.

var maxOSLogArgumentCount: UInt8

The maximum number of interpolated expressions that a log message may contain.

## Relationships

### Conforms To

- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral

## See Also

### Logging a Message

func log(OSLogMessage)

Writes a message to the log using the default log type.

func log(level: OSLogType, OSLogMessage)

Writes a message to the log using the specified log type.

struct OSLogType

The various log levels that the unified logging system provides.

