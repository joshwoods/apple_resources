

- AVFoundation
- AVSampleBufferVideoRenderer
-  flush(removingDisplayedImage:completionHandler:) 

Instance Method

# flush(removingDisplayedImage:completionHandler:)

Tells the video renderer to discard pending enqueued sample buffers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func flush(
    removingDisplayedImage removeDisplayedImage: Bool,
    completionHandler handler: (() -> Void)? = nil
)
```

``` source
func flush(removingDisplayedImage removeDisplayedImage: Bool) async
```

## Parameters 

`removeDisplayedImage`  

A Boolean value that indicates whether to remove the display image.

`handler`  

A completion handler the system invokes when the flush completes.

## See Also

### Flushing the renderer

var requiresFlushToResumeDecoding: Bool

A Boolean value that Indicates whether the renderer requires flushing to continue decoding frames.

class let requiresFlushToResumeDecodingDidChangeNotification: NSNotification.Name

A notification that indicates that the video renderer requires flushing to continue rendering sample buffers.

