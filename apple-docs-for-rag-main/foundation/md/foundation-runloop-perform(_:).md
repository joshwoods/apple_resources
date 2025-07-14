

- Foundation
- RunLoop
-  perform(\_:) 

Instance Method

# perform(\_:)

Schedules a block that the run loop invokes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func perform(_ block: @escaping () -> Void)
```

## Parameters 

`block`  

A block that the run loop invokes.

## See Also

### Scheduling and Canceling Tasks

func perform(inModes: [RunLoop.Mode], block: () -> Void)

Schedules a block that the run loop invokes when it’s running in any of the specified modes.

func perform(Selector, target: Any, argument: Any?, order: Int, modes: [RunLoop.Mode])

Schedules the sending of a message on the receiver.

func cancelPerform(Selector, target: Any, argument: Any?)

Cancels the sending of a previously scheduled message.

func cancelPerformSelectors(withTarget: Any)

Cancels all outstanding ordered performs scheduled with a given target.

