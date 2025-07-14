

- Foundation
- RunLoop
-  add(\_:forMode:) 

Instance Method

# add(\_:forMode:)

Registers a given timer with a given input mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func add(
    _ timer: Timer,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`timer`  

The timer to register with the receiver.

`mode`  

The mode in which to add `aTimer`. You may specify a custom mode or use one of the modes listed in `Run Loop Modes`.

## Discussion

You can add a timer to multiple input modes. While running in the designated mode, the receiver causes the timer to fire on or after its scheduled fire date. Upon firing, the timer invokes its associated handler routine, which is a selector on a designated object.

The receiver retains `aTimer`. To remove a timer from all run loop modes on which it is installed, send an invalidate() message to the timer.

