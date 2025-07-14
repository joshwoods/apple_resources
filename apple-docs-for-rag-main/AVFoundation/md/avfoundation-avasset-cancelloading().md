

- AVFoundation
- AVAsset
-  cancelLoading() 

Instance Method

# cancelLoading()

Cancels all pending requests to asynchronously load property values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func cancelLoading()
```

## Discussion

Calling this method cancels pending requests to load an asset’s property values. Call this method only when you’re done using an asset and you want to cancel any outstanding requests. Deallocating an asset implicitly calls this method if loading requests are still pending.

