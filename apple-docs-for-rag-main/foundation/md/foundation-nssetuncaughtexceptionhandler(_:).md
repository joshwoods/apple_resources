

- Foundation
-  NSSetUncaughtExceptionHandler(\_:) 

Function

# NSSetUncaughtExceptionHandler(\_:)

Changes the top-level error handler.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSSetUncaughtExceptionHandler(_: ((NSException) -> Void)?)
```

## Discussion

Sets the top-level error-handling function where you can perform last-minute logging before the program terminates.

## See Also

### Related Documentation

func NSGetUncaughtExceptionHandler() -> ((NSException) -> Void)?

Returns the top-level error handler.

@MainActor func reportException(_ exception: NSException)

Logs a given exception by calling \`NSLog()\`.

### Functions

func NSGetUncaughtExceptionHandler() -> ((NSException) -> Void)?

Returns the top-level error handler.

