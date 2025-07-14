

- AppKit
- NSRunningApplication
-  forceTerminate() 

Instance Method

# forceTerminate()

Attempts to force the receiver to quit.

macOS 10.6+

``` source
func forceTerminate() -> Bool
```

## Return Value

Returns true if the application successfully terminated, otherwise false.

## Discussion

This method will return false if the application is no longer running when the `forceTerminate` message is sent to the receiver.

This method may return before the receiver exits; you should observe the terminated property to determine when the application terminates.

Sandboxed applications can’t use this method to terminate other applciations. This method returns false when called from a sandboxed application.

## See Also

### Terminating applications

func terminate() -> Bool

Attempts to quit the receiver normally.

var isTerminated: Bool

Indicates that the receiver’s application has terminated.

class func terminateAutomaticallyTerminableApplications()

Terminates invisibly running applications as if triggered by system memory pressure.

