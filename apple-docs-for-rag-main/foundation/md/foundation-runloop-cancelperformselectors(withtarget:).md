

- Foundation
- RunLoop
-  cancelPerformSelectors(withTarget:) 

Instance Method

# cancelPerformSelectors(withTarget:)

Cancels all outstanding ordered performs scheduled with a given target.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancelPerformSelectors(withTarget target: Any)
```

## Parameters 

`target`  

The previously-specified target.

## Discussion

This method cancels the previously scheduled messages associated with the target, ignoring the selector and argument of the scheduled operation. This is in contrast to cancelPerform(_:target:argument:), which requires you to match the selector and argument as well as the target. This method removes the perform requests for the object from all modes of the run loop.

## See Also

### Scheduling and Canceling Tasks

func perform(() -> Void)

Schedules a block that the run loop invokes.

func perform(inModes: [RunLoop.Mode], block: () -> Void)

Schedules a block that the run loop invokes when it’s running in any of the specified modes.

func perform(Selector, target: Any, argument: Any?, order: Int, modes: [RunLoop.Mode])

Schedules the sending of a message on the receiver.

func cancelPerform(Selector, target: Any, argument: Any?)

Cancels the sending of a previously scheduled message.

