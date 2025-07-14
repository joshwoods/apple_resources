

- Foundation
-  NSGetUncaughtExceptionHandler() 

Function

# NSGetUncaughtExceptionHandler()

Returns the top-level error handler.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSGetUncaughtExceptionHandler() -> ((NSException) -> Void)?
```

## Return Value

A pointer to the top-level error-handling function where you can perform last-minute logging before the program terminates.

## See Also

### Related Documentation

func NSSetUncaughtExceptionHandler(((NSException) -> Void)?)

Changes the top-level error handler.

### Functions

func NSSetUncaughtExceptionHandler(((NSException) -> Void)?)

Changes the top-level error handler.

