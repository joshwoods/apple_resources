

- os
- Logger
-  error(\_:) 

Instance Method

# error(\_:)

Writes information about an error to the log.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func error(_ message: OSLogMessage)
```

## Parameters 

`message`  

The interpolated string that the logger writes to the log. Each of the message’s interpolations can specify individual formatting and privacy options. For more information, see Message Argument Formatters.

## Discussion

Important

Don’t create an instance of OSLogMessage. Instead, provide an interpolated string as the `message` parameter and the system converts it automatically.

Use this method to write messages with the error log level to both the in-memory and on-disk log stores.

## See Also

### Logging a Scoped Message

func notice(OSLogMessage)

Writes a message to the log using the default log type.

func debug(OSLogMessage)

Writes a debug message to the log.

func trace(OSLogMessage)

Writes a trace message to the log.

func info(OSLogMessage)

Writes an informative message to the log.

func warning(OSLogMessage)

Writes information about a warning to the log.

func fault(OSLogMessage)

Writes a message to the log about a bug that occurs when your app executes.

func critical(OSLogMessage)

Writes a message to the log about a critical event in your app’s execution.

