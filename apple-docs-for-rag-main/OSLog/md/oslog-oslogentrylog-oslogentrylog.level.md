

- OSLog
- OSLogEntryLog
-  OSLogEntryLog.Level 

Enumeration

# OSLogEntryLog.Level

The log level at which the entry was generated.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Level
```

## Topics

### Log Levels

case undefined

The log level was never specified.

case debug

A log level that captures diagnostic information.

case info

The log level that captures additional information.

case notice

The log level that captures notifications.

case error

The log level that captures errors.

case fault

The log level that captures fault information.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Log Levels

var level: OSLogEntryLog.Level

The log level of the entry.

