

- Exception Handling
-  NSHandleUncaughtSystemExceptionMask 

Global Variable

# NSHandleUncaughtSystemExceptionMask

The exception handler handles uncaught system exceptions by converting them to NSException objects containing a stack trace.

Mac Catalyst 13.0+macOS 10.0+

``` source
var NSHandleUncaughtSystemExceptionMask: Int { get }
```

## See Also

### Constants

var NSLogUncaughtExceptionMask: Int

The exception handler logs uncaught exceptions.

var NSHandleUncaughtExceptionMask: Int

The exception handler handles uncaught exceptions by terminating the thread in which they occur.

var NSLogUncaughtSystemExceptionMask: Int

The exception handler logs uncaught system exceptions.

var NSLogUncaughtRuntimeErrorMask: Int

The exception handler logs uncaught runtime errors.

var NSHandleUncaughtRuntimeErrorMask: Int

The exception handler handles uncaught runtime errors by converting them to NSException objects containing a stack trace.

var NSLogTopLevelExceptionMask: Int

The exception handler logs exceptions that would be caught by the top-level handler.

var NSHandleTopLevelExceptionMask: Int

The exception handler handles exceptions caught by the top-level handler by converting them to NSException objects containing a stack trace.

var NSLogOtherExceptionMask: Int

The exception handler logs exceptions caught by handlers lower than the top-level handler.

var NSHandleOtherExceptionMask: Int

The exception handler handles exceptions caught by handlers lower than the top-level handler by converting them to NSException objects containing a stack trace.

