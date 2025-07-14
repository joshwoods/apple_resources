

- Foundation
- NSMachPort
-  schedule(in:forMode:) 

Instance Method

# schedule(in:forMode:)

Schedules the receiver into the run loop mode `mode` of `runLoop`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func schedule(
    in runLoop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`runLoop`  

The run loop to which to add the receiver.

`mode`  

The run loop mode in which to add the receiver.

## Discussion

When the receiver is scheduled, the run loop monitors the mach port for incoming messages and, when a message arrives, invokes the delegate method handleMachMessage(_:).

## See Also

### Scheduling the Port on a Run Loop

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the receiver from the run loop mode `mode` of `runLoop`.

