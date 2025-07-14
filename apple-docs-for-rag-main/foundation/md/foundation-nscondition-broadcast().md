

- Foundation
- NSCondition
-  broadcast() 

Instance Method

# broadcast()

Signals the condition, waking up all threads waiting on it.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func broadcast()
```

## Discussion

If no threads are waiting on the condition, this method does nothing.

To avoid race conditions, you should invoke this method only while the receiver is locked.

## See Also

### Signaling Waiting Threads

func signal()

Signals the condition, waking up one thread waiting on it.

