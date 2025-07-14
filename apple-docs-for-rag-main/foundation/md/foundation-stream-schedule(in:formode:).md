

- Foundation
- Stream
-  schedule(in:forMode:) 

Instance Method

# schedule(in:forMode:)

Schedules the receiver on a given run loop in a given mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func schedule(
    in aRunLoop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`aRunLoop`  

The run loop on which to schedule the receiver.

`mode`  

The mode for the run loop.

## Discussion

Unless the client is polling the stream, it is responsible for ensuring that the stream is scheduled on at least one run loop and that at least one of the run loops on which the stream is scheduled is being run.

## See Also

### Managing Run Loops

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the receiver from a given run loop running in a given mode.

