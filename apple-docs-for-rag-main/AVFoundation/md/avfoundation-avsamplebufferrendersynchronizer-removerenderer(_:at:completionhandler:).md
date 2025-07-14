

- AVFoundation
- AVSampleBufferRenderSynchronizer
-  removeRenderer(\_:at:completionHandler:) 

Instance Method

# removeRenderer(\_:at:completionHandler:)

Removes a renderer from the synchronizer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func removeRenderer(
    _ renderer: any AVQueuedSampleBufferRendering,
    at time: CMTime,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
func removeRenderer(
    _ renderer: any AVQueuedSampleBufferRendering,
    at time: CMTime
) async -> Bool
```

## Parameters 

`renderer`  

`time`  

The time on the timebase’s timeline at which the renderer should be removed. If the time is in the past, the renderer is immediately removed.

`completionHandler`  

An optional block to invoke when the renderer is removed from the synchronizer. The block takes one argument:

didRemoveRenderer  
A Boolean value indicating the whether the renderer was removed.

## Discussion

This method removes the renderer asynchronously. The method can be called more than once, with a subsequent scheduled removal replacing a previously scheduled removal. This method can be called while rate is not `0.0`.

Clients may provide an optional `completionHandler` to be notified when the scheduled removal is complete. If provided, the completion handler will always be called with the following values for `didRemoveRenderer`:

- If the renderer has not been added to this synchronizer, `didRemoveRenderer` is `NO`.

- If the removal of a particular renderer is scheduled after the same renderer’s removal was previous scheduled but not yet occurred, the previously scheduled removal’s completion handler is and `didRemoveRenderer` set to `NO`.

- When the renderer is removed due to a scheduled removal, the completion handler is called and `didRemoveRenderer` set to YES.

## See Also

### Managing Renderers

var renderers: [any AVQueuedSampleBufferRendering]

An array of queued sample buffer renderers currently attached to the synchronizer.

func addRenderer(any AVQueuedSampleBufferRendering)

Adds a renderer to the list of renderers under the synchronizer’s control.

