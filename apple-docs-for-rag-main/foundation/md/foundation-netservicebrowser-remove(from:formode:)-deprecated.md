

- Foundation
- NetServiceBrowser
-  remove(from:forMode:) Deprecated

Instance Method

# remove(from:forMode:)

Removes the receiver from the specified run loop.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func remove(
    from aRunLoop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

Deprecated

Use nw_browser_t in Network framework instead

## Parameters 

`aRunLoop`  

Run loop from which to remove the receiver.

`mode`  

Run loop mode in which to perform this operation, such as default. See the Run Loop Modes section of the RunLoop class for other run loop mode values.

## Discussion

You can use this method in conjunction with schedule(in:forMode:) to transfer the receiver to a run loop other than the default one. Although it is possible to remove an `NSNetService` object completely from any run loop and then attempt actions on it, you must not do it.

## See Also

### Managing Run Loops

func schedule(in: RunLoop, forMode: RunLoop.Mode)

Adds the receiver to the specified run loop.

Deprecated

