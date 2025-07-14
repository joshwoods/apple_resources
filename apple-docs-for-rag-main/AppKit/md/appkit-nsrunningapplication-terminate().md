

- AppKit
- NSRunningApplication
-  terminate() 

Instance Method

# terminate()

Attempts to quit the receiver normally.

macOS 10.6+

``` source
func terminate() -> Bool
```

## Return Value

Returns true if the request was successfully sent, otherwise false.

## Discussion

This method will return false if the application is no longer running when the terminate message is sent to the receiver.

This method may return before the receiver exits; you should observe the terminated property to determine when the application terminates.

Sandboxed applications can’t use this method to terminate other applications. This method returns false when called from a sandboxed application.

## See Also

### Terminating applications

func forceTerminate() -> Bool

Attempts to force the receiver to quit.

var isTerminated: Bool

Indicates that the receiver’s application has terminated.

class func terminateAutomaticallyTerminableApplications()

Terminates invisibly running applications as if triggered by system memory pressure.

