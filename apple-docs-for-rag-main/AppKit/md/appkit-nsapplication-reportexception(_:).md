

- AppKit
- NSApplication
-  reportException(\_:) 

Instance Method

# reportException(\_:)

Logs a given exception by calling `NSLog()`.

macOS

``` source
@MainActor
func reportException(_ exception: NSException)
```

## Parameters 

`exception`  

The exception whose contents you want to write to the log file.

## Discussion

This method doesn’t raise `anException`. Use it inside of an exception handler to record that the exception occurred.

## See Also

### Related Documentation

func NSSetUncaughtExceptionHandler(((NSException) -> Void)?)

Changes the top-level error handler.

