

- Foundation
- NetService
-  remove(from:forMode:) Deprecated

Instance Method

# remove(from:forMode:)

Removes the service from the given run loop for a given mode.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func remove(
    from aRunLoop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Parameters 

`aRunLoop`  

The run loop from which to remove the receiver.

`mode`  

The run loop mode from which to remove the receiver. Possible values for `mode` are discussed in the “Constants” section of RunLoop.

## Discussion

You can use this method in conjunction with schedule(in:forMode:) to transfer the service to a different run loop. Although it is possible to remove an `NSNetService` object completely from any run loop and then attempt actions on it, it is an error to do so.

## See Also

### Managing Run Loops

func schedule(in: RunLoop, forMode: RunLoop.Mode)

Adds the service to the specified run loop.

Deprecated

