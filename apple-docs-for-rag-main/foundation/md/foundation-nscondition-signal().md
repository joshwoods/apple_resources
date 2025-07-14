

- Foundation
- NSCondition
-  signal() 

Instance Method

# signal()

Signals the condition, waking up one thread waiting on it.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func signal()
```

## Discussion

You use this method to wake up one thread that is waiting on the condition. You may call this method multiple times to wake up multiple threads. If no threads are waiting on the condition, this method does nothing.

To avoid race conditions, you should invoke this method only while the receiver is locked.

## See Also

### Signaling Waiting Threads

func broadcast()

Signals the condition, waking up all threads waiting on it.

