

- Foundation
- Thread
-  cancel() 

Instance Method

# cancel()

Changes the cancelled state of the receiver to indicate that it should exit.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancel()
```

## Discussion

The semantics of this method are the same as those used for Operation. This method sets state information in the receiver that is then reflected by the isCancelled property. Threads that support cancellation should periodically call the isCancelled method to determine if the thread has in fact been cancelled, and exit if it has been.

For more information about cancellation and operation objects, see Operation.

## See Also

### Related Documentation

var isCancelled: Bool

A Boolean value that indicates whether the receiver is cancelled.

### Stopping a Thread

class func sleep(until: Date)

Blocks the current thread until the time specified.

class func sleep(forTimeInterval: TimeInterval)

Sleeps the thread for a given time interval.

class func exit()

Terminates the current thread.

