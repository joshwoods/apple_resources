

- os
- OSLogType
-  debug 

Type Property

# debug

The debug log level.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
static let debug: OSLogType
```

## Discussion

Logging a message of this type is equivalent to calling the os_log_debug function. Use this level to capture information that may be useful during development or while troubleshooting a specific problem.

The system only captures debug-level messages in memory when you enable debug logging through a configuration change, and purges them in accordance with the configuration’s persistence setting.

## See Also

### Getting Log Types

static let info: OSLogType

The informative log level.

static let `default`: OSLogType

The default log level.

static let error: OSLogType

The error log level.

static let fault: OSLogType

The fault log level.

