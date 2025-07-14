

- os
- OSLog
-  disabled 

Type Property

# disabled

The shared disabled log.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
static let disabled: OSLog
```

## Discussion

Passing this constant to an `os_log` function prevents the system from logging a message.

## See Also

### Getting the Shared Logs

static let `default`: OSLog

The shared default log.

