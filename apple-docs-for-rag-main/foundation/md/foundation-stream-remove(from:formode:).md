

- Foundation
- Stream
-  remove(from:forMode:) 

Instance Method

# remove(from:forMode:)

Removes the receiver from a given run loop running in a given mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remove(
    from aRunLoop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`aRunLoop`  

The run loop on which the receiver was scheduled.

`mode`  

The mode for the run loop.

## See Also

### Managing Run Loops

func schedule(in: RunLoop, forMode: RunLoop.Mode)

Schedules the receiver on a given run loop in a given mode.

