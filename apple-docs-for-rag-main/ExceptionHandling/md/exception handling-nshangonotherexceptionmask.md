

- Exception Handling
-  NSHangOnOtherExceptionMask 

Global Variable

# NSHangOnOtherExceptionMask

The exception handler suspends execution when it detects an exception that would be handled by an object other than the top-level handler.

Mac Catalyst 13.0+macOS 10.0+

``` source
var NSHangOnOtherExceptionMask: Int { get }
```

## See Also

### Constants

var NSHangOnUncaughtExceptionMask: Int

The exception handler suspends execution when it detects an uncaught exception (other than a system exception or runtime error).

var NSHangOnUncaughtSystemExceptionMask: Int

The exception handler suspends execution when it detects an uncaught system exception.

var NSHangOnUncaughtRuntimeErrorMask: Int

The exception handler suspends execution when it detects an uncaught runtime error.

var NSHangOnTopLevelExceptionMask: Int

The exception handler suspends execution when it detects an exception that would be handled by the top-level handler.

