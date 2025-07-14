

- AVFoundation
- AVAssetWriterInput
-  requestMediaDataWhenReady(on:using:) 

Instance Method

# requestMediaDataWhenReady(on:using:)

Tells the input to request media data, at its convenience, to write to the output file.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func requestMediaDataWhenReady(
    on queue: dispatch_queue_t,
    using block: @escaping () -> Void
)
```

## Parameters 

`queue`  

The queue on which the system invokes the callback.

`block`  

A callback that the input invokes to retrieve additional media data.

## Discussion

Use this method when working with pull-style buffer sources, such as an AVAssetReaderOutput. The callback you provide appends media data to the input until its isReadyForMoreMediaData property becomes false, or when there’s no more media data to process (at which point you may mark the input as finished by calling its markAsFinished() method). If you don’t mark the input as finished, after the input processes the media data and becomes ready for more, it invokes the callback again to append more data. The example below shows a typical callback implementation.

```
let serialQueue = DispatchQueue(label: "RequestMedia")
assetWriterInput?.requestMediaDataWhenReady(on: serialQueue) { [weak self] in
    guard let self = self,
          let assetWriterInput = self.assetWriterInput else { return }
    while self.assetWriterInput!.isReadyForMoreMediaData {
        // Copy the next sample buffer from your source media.
        guard let nextSampleBuffer = copyNextSampleBufferToWrite() else {
            // Mark the input as finished.
            self.assetWriterInput!.markAsFinished()
            break
        }
        // Append the sample buffer to the input.
        self.assetWriterInput!.append(nextSampleBuffer)
    }      
}
```

When working with push-style sources, such as an AVCaptureAudioDataOutput or AVCaptureVideoDataOutput, append buffers directly to the asset writer input when you receive them using its append(_:) method. Using this method helps avoid having to queue up buffers in between the buffer source and the asset writer input.

## See Also

### Appending Media Samples

var expectsMediaDataInRealTime: Bool

A Boolean value that indicates whether the input tailors its processing for real-time sources.

var isReadyForMoreMediaData: Bool

A Boolean value that indicates whether the input is ready to accept media data.

func append(CMSampleBuffer) -> Bool

Appends a sample buffer to an input to write to the output file.

func markAsFinished()

Marks the input as finished to indicate that you’re done appending samples to it.

