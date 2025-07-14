

- Foundation
- NetServiceBrowser
-  schedule(in:forMode:) Deprecated

Instance Method

# schedule(in:forMode:)

Adds the receiver to the specified run loop.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func schedule(
    in aRunLoop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

Deprecated

Use nw_browser_t in Network framework instead

## Parameters 

`aRunLoop`  

Run loop in which to schedule the receiver.

`mode`  

Run loop mode in which to perform this operation, such as default. See the Run Loop Modes section of the RunLoop class for other run loop mode values.

## Discussion

You can use this method in conjunction with remove(from:forMode:) to transfer the receiver to a run loop other than the default one. You should not attempt to run the receiver on multiple run loops.

## See Also

### Managing Run Loops

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the receiver from the specified run loop.

Deprecated

