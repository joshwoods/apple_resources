

- Foundation
- Thread
-  exit() 

Type Method

# exit()

Terminates the current thread.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func exit()
```

## Discussion

This method uses the current class method to access the current thread. Before exiting the thread, this method posts the NSThreadWillExit with the thread being exited to the default notification center. Because notifications are delivered synchronously, all observers of NSThreadWillExit are guaranteed to receive the notification before the thread exits.

Invoking this method should be avoided as it does not give your thread a chance to clean up any resources it allocated during its execution.

## See Also

### Related Documentation

class var current: Thread

Returns the thread object representing the current thread of execution.

### Stopping a Thread

class func sleep(until: Date)

Blocks the current thread until the time specified.

class func sleep(forTimeInterval: TimeInterval)

Sleeps the thread for a given time interval.

func cancel()

Changes the cancelled state of the receiver to indicate that it should exit.

