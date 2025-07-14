

- Objective-C Runtime
- NSObject
-  exceptionHandler(\_:shouldLogException:mask:) 

Instance Method

# exceptionHandler(\_:shouldLogException:mask:)

Implemented by the delegate to evaluate whether the delegating exception hangler should log a given exception.

macOS

``` source
func exceptionHandler(
    _ sender: NSExceptionHandler!,
    shouldLogException exception: NSException!,
    mask aMask: Int
) -> Bool
```

## Parameters 

`sender`  

The NSExceptionHandler object sending the message.

`exception`  

An NSException object describing the exception to be evaluated.

`aMask`  

The bit mask indicating the types of exceptions logged by the NSExceptionHandler object. See Logging and Handling Constants and System Hang Constants for descriptions of the possible `enum` constants.

## Return Value

YES to have the NSExceptionHandler object log the exception, NO otherwise.

