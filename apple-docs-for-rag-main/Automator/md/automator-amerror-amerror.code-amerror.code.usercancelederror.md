

- Automator
- AMError
- AMError.Code
-  AMError.Code.userCanceledError 

Case

# AMError.Code.userCanceledError

An error that indicates the user cancelled.

Mac Catalyst 14.0+macOS 10.4+

``` source
case userCanceledError
```

## Discussion

This error is the same as the AppleScript error userCanceledErr. When an Apple Event is canceled by the user, a running action may return this error. Automator ignores the error and stops the workflow gracefully, without displaying the error to the user.

