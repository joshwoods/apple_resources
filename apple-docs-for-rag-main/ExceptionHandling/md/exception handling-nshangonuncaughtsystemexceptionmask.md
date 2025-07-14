

- Exception Handling
-  NSHangOnUncaughtSystemExceptionMask 

Global Variable

# NSHangOnUncaughtSystemExceptionMask

The exception handler suspends execution when it detects an uncaught system exception.

Mac Catalyst 13.0+macOS 10.0+

``` source
var NSHangOnUncaughtSystemExceptionMask: Int { get }
```

## See Also

### Constants

var NSHangOnUncaughtExceptionMask: Int

The exception handler suspends execution when it detects an uncaught exception (other than a system exception or runtime error).

var NSHangOnUncaughtRuntimeErrorMask: Int

The exception handler suspends execution when it detects an uncaught runtime error.

var NSHangOnTopLevelExceptionMask: Int

The exception handler suspends execution when it detects an exception that would be handled by the top-level handler.

var NSHangOnOtherExceptionMask: Int

The exception handler suspends execution when it detects an exception that would be handled by an object other than the top-level handler.

