

- Foundation
- RunLoop
-  perform(inModes:block:) 

Instance Method

# perform(inModes:block:)

Schedules a block that the run loop invokes when it’s running in any of the specified modes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func perform(
    inModes modes: [RunLoop.Mode],
    block: @escaping () -> Void
)
```

## Parameters 

`modes`  

An array of modes in which the run loop invokes the block.

`block`  

The block that the run loop invokes.

## See Also

### Scheduling and Canceling Tasks

func perform(() -> Void)

Schedules a block that the run loop invokes.

func perform(Selector, target: Any, argument: Any?, order: Int, modes: [RunLoop.Mode])

Schedules the sending of a message on the receiver.

func cancelPerform(Selector, target: Any, argument: Any?)

Cancels the sending of a previously scheduled message.

func cancelPerformSelectors(withTarget: Any)

Cancels all outstanding ordered performs scheduled with a given target.

