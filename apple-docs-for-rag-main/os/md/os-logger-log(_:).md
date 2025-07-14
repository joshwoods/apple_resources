

- os
- Logger
-  log(\_:) 

Instance Method

# log(\_:)

Writes a message to the log using the default log type.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func log(_ message: OSLogMessage)
```

## Parameters 

`message`  

The interpolated string that the logger writes to the log. Each of the message’s interpolations can specify individual formatting and privacy options. For more information, see Message Argument Formatters.

## Discussion

Important

Don’t create an instance of OSLogMessage. Instead, provide an interpolated string as the `message` parameter and the system converts it automatically.

Use this method to write messages using the default log level to both the in-memory and on-disk log stores. This method is functionally equivalent to the notice(_:) method.

## See Also

### Logging a Message

func log(level: OSLogType, OSLogMessage)

Writes a message to the log using the specified log type.

struct OSLogType

The various log levels that the unified logging system provides.

struct OSLogMessage

An object that represents a log message.

