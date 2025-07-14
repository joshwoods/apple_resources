

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  renderers 

Instance Property

# renderers

An array of queued sample buffer renderers currently attached to the synchronizer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var renderers: [any AVQueuedSampleBufferRendering] { get }
```

## Discussion

This property includes all renderers that have been added to the synchronizer and haven’t been removed, including renderers that have been scheduled for removal, but have yet to be removed. This property is not KVO observable.

## See Also

### Managing Renderers

func addRenderer(any AVQueuedSampleBufferRendering)

Adds a renderer to the list of renderers under the synchronizer’s control.

func removeRenderer(any AVQueuedSampleBufferRendering, at: CMTime, completionHandler: ((Bool) -> Void)?)

Removes a renderer from the synchronizer.

