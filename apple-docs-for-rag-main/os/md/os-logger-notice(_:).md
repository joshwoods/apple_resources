

- os
- Logger
-  notice(\_:) 

Instance Method

# notice(\_:)

Writes a message to the log using the default log type.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func notice(_ message: OSLogMessage)
```

## Parameters 

`message`  

The interpolated string that the logger writes to the log. Each of the message’s interpolations can specify individual formatting and privacy options. For more information, see Message Argument Formatters.

## Discussion

Important

Don’t create an instance of OSLogMessage. Instead, provide an interpolated string as the `message` parameter and the system converts it automatically.

This method is functionally equivalent to the log(_:) method.

## See Also

### Logging a Scoped Message

func debug(OSLogMessage)

Writes a debug message to the log.

func trace(OSLogMessage)

Writes a trace message to the log.

func info(OSLogMessage)

Writes an informative message to the log.

func error(OSLogMessage)

Writes information about an error to the log.

func warning(OSLogMessage)

Writes information about a warning to the log.

func fault(OSLogMessage)

Writes a message to the log about a bug that occurs when your app executes.

func critical(OSLogMessage)

Writes a message to the log about a critical event in your app’s execution.

