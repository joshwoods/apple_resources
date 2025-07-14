

- os
- Logger
-  log(level:\_:) 

Instance Method

# log(level:\_:)

Writes a message to the log using the specified log type.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func log(
    level: OSLogType,
    _ message: OSLogMessage
)
```

## Parameters 

`level`  

The message’s log level, which determines the severity of the message and whether the system persists it to disk. For possible values, see OSLogType.

`message`  

The interpolated string that the logger writes to the log. Each of the message’s interpolations can specify individual formatting and privacy options. For more information, see Message Argument Formatters.

## Discussion

Important

Don’t create an instance of OSLogMessage. Instead, provide an interpolated string as the `message` parameter and the system converts it automatically.

## See Also

### Logging a Message

func log(OSLogMessage)

Writes a message to the log using the default log type.

struct OSLogType

The various log levels that the unified logging system provides.

struct OSLogMessage

An object that represents a log message.

