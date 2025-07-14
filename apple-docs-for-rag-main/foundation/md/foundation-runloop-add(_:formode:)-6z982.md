

- Foundation
- RunLoop
-  add(\_:forMode:) 

Instance Method

# add(\_:forMode:)

Adds a port as an input source to the specified mode of the run loop.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func add(
    _ aPort: Port,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`aPort`  

The port to add to the receiver.

`mode`  

The mode in which to add `aPort`. You may specify a custom mode or use one of the modes listed in `Run Loop Modes`.

## Discussion

This method schedules the port with the receiver. You can add a port to multiple input modes. When the receiver is running in the specified mode, it dispatches messages destined for that port to the port’s designated handler routine.

## See Also

### Managing Ports

func remove(Port, forMode: RunLoop.Mode)

Removes a port from the specified input mode of the run loop.

