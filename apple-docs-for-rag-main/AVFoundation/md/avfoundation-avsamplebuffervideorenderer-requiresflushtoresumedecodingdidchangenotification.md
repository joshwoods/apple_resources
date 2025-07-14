

- AVFoundation
- AVSampleBufferVideoRenderer
-  requiresFlushToResumeDecodingDidChangeNotification 

Type Property

# requiresFlushToResumeDecodingDidChangeNotification

A notification that indicates that the video renderer requires flushing to continue rendering sample buffers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class let requiresFlushToResumeDecodingDidChangeNotification: NSNotification.Name
```

## See Also

### Flushing the renderer

var requiresFlushToResumeDecoding: Bool

A Boolean value that Indicates whether the renderer requires flushing to continue decoding frames.

func flush(removingDisplayedImage: Bool, completionHandler: (() -> Void)?)

Tells the video renderer to discard pending enqueued sample buffers.

