

- Foundation
- Port
-  schedule(in:forMode:) 

Instance Method

# schedule(in:forMode:)

This method should be implemented by a subclass to set up monitoring of a port when added to a given run loop in a given input mode.

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

The run loop mode to which to add the receiver

## Discussion

This method should not be called directly.

## See Also

### Port Monitoring

func remove(from: RunLoop, forMode: RunLoop.Mode)

This method should be implemented by a subclass to stop monitoring of a port when removed from a give run loop in a given input mode.

