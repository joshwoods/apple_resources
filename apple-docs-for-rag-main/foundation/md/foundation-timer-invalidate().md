

- Foundation
- Timer
-  invalidate() 

Instance Method

# invalidate()

Stops the timer from ever firing again and requests its removal from its run loop.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func invalidate()
```

## Discussion

This method is the only way to remove a timer from an RunLoop object. The RunLoop object removes its strong reference to the timer, either just before the invalidate() method returns or at some later point.

If it was configured with target and user info objects, the receiver removes its strong references to those objects as well.

### Special Considerations

You must send this message from the thread on which the timer was installed. If you send this message from another thread, the input source associated with the timer may not be removed from its run loop, which could prevent the thread from exiting properly.

## See Also

### Related Documentation

func fire()

Causes the timer’s message to be sent to its target.

