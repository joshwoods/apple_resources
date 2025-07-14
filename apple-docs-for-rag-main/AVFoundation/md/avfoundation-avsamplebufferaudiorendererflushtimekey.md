

- AVFoundation
-  AVSampleBufferAudioRendererFlushTimeKey 

Global Variable

# AVSampleBufferAudioRendererFlushTimeKey

The key that indicates the presentation timestamp of the first queued sample that was flushed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let AVSampleBufferAudioRendererFlushTimeKey: String
```

## Discussion

The value for this key is an NSValue object that wraps a CMTime value.

## See Also

### Removing Queued Buffers

func flush(fromSourceTime: CMTime, completionHandler: (Bool) -> Void)

Flushes queued sample buffers with presentation time stamps later than or equal to the specified time.

