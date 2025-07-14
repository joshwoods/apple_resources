

- AppKit
- NSRunningApplication
-  isTerminated 

Instance Property

# isTerminated

Indicates that the receiver’s application has terminated.

macOS 10.6+

``` source
var isTerminated: Bool { get }
```

## Discussion

The value of terminated is true if the receiver’s application has terminated, otherwise false.

This property is observable using key-value observing.

## See Also

### Terminating applications

func forceTerminate() -> Bool

Attempts to force the receiver to quit.

func terminate() -> Bool

Attempts to quit the receiver normally.

class func terminateAutomaticallyTerminableApplications()

Terminates invisibly running applications as if triggered by system memory pressure.

