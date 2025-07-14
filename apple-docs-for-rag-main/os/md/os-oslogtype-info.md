

- os
- OSLogType
-  info 

Type Property

# info

The informative log level.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
static let info: OSLogType
```

## Discussion

Logging a message of this type is equivalent to calling the os_log_info function. Use this level to capture information that may be helpful, but not essential, for troubleshooting errors.

The system stores info-level messages in memory buffers and, without a configuration change, purges the oldest messages as those buffers fill up. However, the system writes the messages to the data store when faults and, optionally, errors occur. Info-level messages remain in the data store until the store’s size exceeds its storage quota, at which point, the system purges the oldest messages in the data store to free up space.

## See Also

### Getting Log Types

static let debug: OSLogType

The debug log level.

static let `default`: OSLogType

The default log level.

static let error: OSLogType

The error log level.

static let fault: OSLogType

The fault log level.

