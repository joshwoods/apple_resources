

- Objective-C Runtime
- NSObject
-  exceptionHandler(\_:shouldHandle:mask:) 

Instance Method

# exceptionHandler(\_:shouldHandle:mask:)

Implemented by the delegate to evaluate whether the delegating exception handler should handle a given exception.

macOS

``` source
func exceptionHandler(
    _ sender: NSExceptionHandler!,
    shouldHandle exception: NSException!,
    mask aMask: Int
) -> Bool
```

## Parameters 

`sender`  

The NSExceptionHandler object sending the message.

`exception`  

An NSException object describing the exception to be evaluated.

`aMask`  

The bit mask indicating the types of exceptions handled by the NSExceptionHandler object. See Logging and Handling Constants and System Hang Constants for descriptions of the possible `enum` constants.

## Return Value

YES to have the NSExceptionHandler object handle the exception, NO otherwise.

