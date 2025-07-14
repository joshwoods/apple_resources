

- AVFoundation
- AVSampleBufferVideoRenderer
-  requiresFlushToResumeDecoding 

Instance Property

# requiresFlushToResumeDecoding

A Boolean value that Indicates whether the renderer requires flushing to continue decoding frames.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var requiresFlushToResumeDecoding: Bool { get }
```

## Discussion

When your app enters a state where using a video decoder resources is not permissible, the value of this property changes to true along with the video renderer’s status changing to AVQueuedSampleBufferRenderingStatus.failed. To resume rendering sample buffers, you must first reset the video renderer by calling flush() or flush(removingDisplayedImage:completionHandler:).

This property is not key-value observable. Instead, track changes to this property by observing notifications of type requiresFlushToResumeDecodingDidChangeNotification.

## See Also

### Flushing the renderer

class let requiresFlushToResumeDecodingDidChangeNotification: NSNotification.Name

A notification that indicates that the video renderer requires flushing to continue rendering sample buffers.

func flush(removingDisplayedImage: Bool, completionHandler: (() -> Void)?)

Tells the video renderer to discard pending enqueued sample buffers.

