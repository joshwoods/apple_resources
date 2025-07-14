

- Foundation
- NSMachPort
-  remove(from:forMode:) 

Instance Method

# remove(from:forMode:)

Removes the receiver from the run loop mode `mode` of `runLoop`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remove(
    from runLoop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`runLoop`  

The run loop from which to remove the receiver.

`mode`  

The run loop mode from which to remove the receiver.

## Discussion

When the receiver is removed, the run loop stops monitoring the Mach port for incoming messages.

## See Also

### Scheduling the Port on a Run Loop

func schedule(in: RunLoop, forMode: RunLoop.Mode)

Schedules the receiver into the run loop mode `mode` of `runLoop`.

