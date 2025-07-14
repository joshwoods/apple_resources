

- Exception Handling
-  NSExceptionHandlerDelegate 

# NSExceptionHandlerDelegate

The `NSExceptionHandlerDelegate` informal protocol describes methods that NSExceptionHandler objects call on their delegates when exceptions occur. An NSExceptionHandler object does not need to have a delegate. When one does, these delegate methods are asked to approve exception handling and logging for each monitored NSExceptionHandler object.

## Topics

### Logging and handling exceptions

func exceptionHandler(_ sender: NSExceptionHandler!, shouldHandle exception: NSException!, mask aMask: Int) -> Bool

Implemented by the delegate to evaluate whether the delegating exception handler should handle a given exception.

func exceptionHandler(_ sender: NSExceptionHandler!, shouldLogException exception: NSException!, mask aMask: Int) -> Bool

Implemented by the delegate to evaluate whether the delegating exception hangler should log a given exception.

