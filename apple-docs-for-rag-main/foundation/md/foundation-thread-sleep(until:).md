

- Foundation
- Thread
-  sleep(until:) 

Type Method

# sleep(until:)

Blocks the current thread until the time specified.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func sleep(until date: Date)
```

## Parameters 

`date`  

The time at which to resume processing.

## Discussion

No run loop processing occurs while the thread is blocked.

## See Also

### Related Documentation

class var current: Thread

Returns the thread object representing the current thread of execution.

### Stopping a Thread

class func sleep(forTimeInterval: TimeInterval)

Sleeps the thread for a given time interval.

class func exit()

Terminates the current thread.

func cancel()

Changes the cancelled state of the receiver to indicate that it should exit.

