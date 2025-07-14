

- AppKit
- NSRunningApplication
-  terminateAutomaticallyTerminableApplications() 

Type Method

# terminateAutomaticallyTerminableApplications()

Terminates invisibly running applications as if triggered by system memory pressure.

macOS 10.6+

``` source
class func terminateAutomaticallyTerminableApplications()
```

## Discussion

This method is intended for installer applications and similar applications to ensure that nothing is unexpectedly relying on the files they’re replacing.

## See Also

### Terminating applications

func forceTerminate() -> Bool

Attempts to force the receiver to quit.

func terminate() -> Bool

Attempts to quit the receiver normally.

var isTerminated: Bool

Indicates that the receiver’s application has terminated.

