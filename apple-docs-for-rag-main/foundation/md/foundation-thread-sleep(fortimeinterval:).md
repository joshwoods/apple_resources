

- Foundation
- Thread
-  sleep(forTimeInterval:) 

Type Method

# sleep(forTimeInterval:)

Sleeps the thread for a given time interval.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func sleep(forTimeInterval ti: TimeInterval)
```

## Parameters 

`ti`  

The duration of the sleep.

## Discussion

No run loop processing occurs while the thread is blocked.

## See Also

### Stopping a Thread

class func sleep(until: Date)

Blocks the current thread until the time specified.

class func exit()

Terminates the current thread.

func cancel()

Changes the cancelled state of the receiver to indicate that it should exit.

