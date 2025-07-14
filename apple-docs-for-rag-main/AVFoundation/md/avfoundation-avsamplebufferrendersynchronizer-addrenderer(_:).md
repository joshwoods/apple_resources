

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  addRenderer(\_:) 

Instance Method

# addRenderer(\_:)

Adds a renderer to the list of renderers under the synchronizer’s control.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func addRenderer(_ renderer: any AVQueuedSampleBufferRendering)
```

## Parameters 

`renderer`  

The render to be added.

## Discussion

This method can be called while rate is not `0.0`.

## See Also

### Managing Renderers

var renderers: [any AVQueuedSampleBufferRendering]

An array of queued sample buffer renderers currently attached to the synchronizer.

func removeRenderer(any AVQueuedSampleBufferRendering, at: CMTime, completionHandler: ((Bool) -> Void)?)

Removes a renderer from the synchronizer.

