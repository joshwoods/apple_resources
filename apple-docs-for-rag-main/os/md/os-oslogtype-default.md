

- os
- OSLogType
-  default 

Type Property

# default

The default log level.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
static let `default`: OSLogType
```

## Discussion

Logging a message of this type is equivalent to calling the os_log function. Use this level to capture information about things that might result in a failure.

The system stores default-level messages in memory buffers and, without a configuration change, compresses the messages and writes them to the data store as those buffers fill up. They remain in the data store until the store’s size exceeds its storage quota, at which point, the system purges the oldest messages in the store to free up space.

## See Also

### Getting Log Types

static let debug: OSLogType

The debug log level.

static let info: OSLogType

The informative log level.

static let error: OSLogType

The error log level.

static let fault: OSLogType

The fault log level.

