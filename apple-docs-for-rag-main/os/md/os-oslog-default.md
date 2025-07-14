

- os
- OSLog
-  default 

Type Property

# default

The shared default log.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
static let `default`: OSLog
```

## Discussion

Passing this constant to an `os_log` function causes the system to log a message with the system’s standard behavior.

## See Also

### Getting the Shared Logs

static let disabled: OSLog

The shared disabled log.

