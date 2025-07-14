

- Exception Handling
- NSExceptionHandler
-  exceptionHangingMask() 

Instance Method

# exceptionHangingMask()

Returns a bit mask representing the types of exceptions that will halt execution for debugging.

Mac Catalyst 13.0+macOS 10.0+

``` source
func exceptionHangingMask() -> Int
```

## Return Value

A bit mask composed of one or more constants specifying the types of exceptions that will halt execution for debugging. See System Hang Constants for information about the constants.

## See Also

### Getting and setting exception masks

func exceptionHandlingMask() -> Int

Returns a bit mask representing the types of exceptions monitored by the receiver and its handling and logging behavior.

func setExceptionHandlingMask(Int)

Sets the bit mask of constants specifying the types of exceptions monitored by the receiver and its handling and logging behavior.

func setExceptionHangingMask(Int)

Sets the bit mask of constants specifying the types of exceptions that will halt execution for debugging.

