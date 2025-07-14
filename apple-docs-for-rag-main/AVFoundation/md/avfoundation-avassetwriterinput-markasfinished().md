

- AVFoundation
- AVAssetWriterInput
-  markAsFinished() 

Instance Method

# markAsFinished()

Marks the input as finished to indicate that you’re done appending samples to it.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func markAsFinished()
```

## Discussion

Apps that monitor an input’s isReadyForMoreMediaData value must call this method when they finish appending to it. This is necessary to prevent other inputs from stalling because they’re waiting on the input’s media data to complete the ideal interleaving pattern.

After calling this method from the serial queue passed to requestMediaDataWhenReady(on:using:), the input issues no more invocations of the callback it passes to that method.

## See Also

### Appending Media Samples

var expectsMediaDataInRealTime: Bool

A Boolean value that indicates whether the input tailors its processing for real-time sources.

var isReadyForMoreMediaData: Bool

A Boolean value that indicates whether the input is ready to accept media data.

func requestMediaDataWhenReady(on: dispatch_queue_t, using: () -> Void)

Tells the input to request media data, at its convenience, to write to the output file.

func append(CMSampleBuffer) -> Bool

Appends a sample buffer to an input to write to the output file.

