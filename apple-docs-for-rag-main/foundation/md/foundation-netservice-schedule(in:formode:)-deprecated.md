

- Foundation
- NetService
-  schedule(in:forMode:) Deprecated

Instance Method

# schedule(in:forMode:)

Adds the service to the specified run loop.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func schedule(
    in aRunLoop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Parameters 

`aRunLoop`  

The run loop to which to add the receiver.

`mode`  

The run loop mode to which to add the receiver. Possible values for `mode` are discussed in the “Constants” section of RunLoop.

## Discussion

You can use this method in conjunction with remove(from:forMode:) to transfer a service to a different run loop. You should not attempt to run a service on multiple run loops.

## See Also

### Managing Run Loops

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the service from the given run loop for a given mode.

Deprecated

