

- Exception Handling
- NSExceptionHandler
-  setExceptionHandlingMask(\_:) 

Instance Method

# setExceptionHandlingMask(\_:)

Sets the bit mask of constants specifying the types of exceptions monitored by the receiver and its handling and logging behavior.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setExceptionHandlingMask(_ aMask: Int)
```

## Parameters 

`aMask`  

A bit mask composed of one or more constants specifying the types of exceptions monitored and whether they are handled or logged (or both). You specify multiple constants by performing a bitwise-OR operation. See Logging and Handling Constants for information about the constants.

## See Also

### Getting and setting exception masks

func exceptionHandlingMask() -> Int

Returns a bit mask representing the types of exceptions monitored by the receiver and its handling and logging behavior.

func exceptionHangingMask() -> Int

Returns a bit mask representing the types of exceptions that will halt execution for debugging.

func setExceptionHangingMask(Int)

Sets the bit mask of constants specifying the types of exceptions that will halt execution for debugging.

