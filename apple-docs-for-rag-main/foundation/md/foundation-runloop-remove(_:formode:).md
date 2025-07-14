

- Foundation
- RunLoop
-  remove(\_:forMode:) 

Instance Method

# remove(\_:forMode:)

Removes a port from the specified input mode of the run loop.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remove(
    _ aPort: Port,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`aPort`  

The port to remove from the receiver.

`mode`  

The mode from which to remove `aPort`. You may specify a custom mode or use one of the modes listed in `Run Loop Modes`.

## Discussion

If you added the port to multiple input modes, you must remove it from each mode separately.

## See Also

### Managing Ports

func add(Port, forMode: RunLoop.Mode)

Adds a port as an input source to the specified mode of the run loop.

