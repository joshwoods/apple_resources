

- Exception Handling
- NSExceptionHandler
-  exceptionHandlingMask() 

Instance Method

# exceptionHandlingMask()

Returns a bit mask representing the types of exceptions monitored by the receiver and its handling and logging behavior.

Mac Catalyst 13.0+macOS 10.0+

``` source
func exceptionHandlingMask() -> Int
```

## Return Value

A bit mask composed of one or more constants specifying the types of exceptions monitored and whether they are handled or logged (or both). See Logging and Handling Constants for information about the constants.

## See Also

### Getting and setting exception masks

func exceptionHangingMask() -> Int

Returns a bit mask representing the types of exceptions that will halt execution for debugging.

func setExceptionHandlingMask(Int)

Sets the bit mask of constants specifying the types of exceptions monitored by the receiver and its handling and logging behavior.

func setExceptionHangingMask(Int)

Sets the bit mask of constants specifying the types of exceptions that will halt execution for debugging.

