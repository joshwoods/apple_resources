

- Metal
-  MTLLogLevel 

Enumeration

# MTLLogLevel

The supported log levels for shader logging.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum MTLLogLevel
```

## Topics

### Enumeration Cases

case debug

The log level that captures diagnostic information.

case info

The log level that captures additional information.

case notice

The log level that captures notifications.

case error

The log level that captures error information.

case fault

The log level that captures fault information.

case undefined

The log level when the log level hasn’t been configured.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

