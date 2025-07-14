

- os
- OSLogType
-  fault 

Type Property

# fault

The fault log level.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
static let fault: OSLogType
```

## Discussion

Logging a message at this level is equivalent to calling the os_log_fault function. Use this level only to capture system-level or multiprocess information when reporting system errors.

The system always writes fault-level messages to the data store. They remain in the store until its size exceeds its storage quota, at which point, the system purges the oldest messages in the store to free up space. If an activity object exists, logging at this level captures information for the entire process chain.

## See Also

### Getting Log Types

static let debug: OSLogType

The debug log level.

static let info: OSLogType

The informative log level.

static let `default`: OSLogType

The default log level.

static let error: OSLogType

The error log level.

