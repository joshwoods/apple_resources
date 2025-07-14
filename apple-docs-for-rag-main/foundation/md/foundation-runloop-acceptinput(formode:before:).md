

- Foundation
- RunLoop
-  acceptInput(forMode:before:) 

Instance Method

# acceptInput(forMode:before:)

Runs the loop once or until the specified date, accepting input only for the specified mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func acceptInput(
    forMode mode: RunLoop.Mode,
    before limitDate: Date
)
```

## Parameters 

`mode`  

The mode in which to run. You may specify custom modes or use one of the modes listed in `Run Loop Modes`.

`limitDate`  

The date up until which to run.

## Discussion

If no input sources or timers are attached to the run loop, this method exits immediately; otherwise, it runs the run loop once, returning as soon as one input source processes a message or the specifed time elapses.

Note

A timer is not considered an input source and may fire multiple times while waiting for this method to return

Manually removing all known input sources and timers from the run loop is not a guarantee that the run loop will exit. macOS can install and remove additional input sources as needed to process requests targeted at the receiver’s thread. Those sources could therefore prevent the run loop from exiting.

## See Also

### Running a Loop

func run()

Puts the receiver into a permanent loop, during which time it processes data from all attached input sources.

func run(mode: RunLoop.Mode, before: Date) -> Bool

Runs the loop once, blocking for input in the specified mode until a given date.

func run(until: Date)

Runs the loop until the specified date, during which time it processes data from all attached input sources.

