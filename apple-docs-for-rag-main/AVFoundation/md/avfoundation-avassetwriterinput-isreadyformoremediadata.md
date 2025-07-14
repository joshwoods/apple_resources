

- AVFoundation
- AVAssetWriterInput
-  isReadyForMoreMediaData 

Instance Property

# isReadyForMoreMediaData

A Boolean value that indicates whether the input is ready to accept media data.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var isReadyForMoreMediaData: Bool { get }
```

## Discussion

An asset writer with multiple inputs writes media data in an interleaved manner for efficient playback and storage. To maintain appropriate interleaving, you can only append data to an input when the value of this property is true.

Apps that write media data from a non-real-time source, such as an instance of AVAssetReader, wait to generate or retrieve more media data while this property value is false. To control of the supply of non-real-time media data, use the requestMediaDataWhenReady(on:using:) method to specify a callback for the input to invoke when it’s ready to append more data.

Apps that write media data from a real-time source, such as an instance of AVCaptureOutput, set the input’s expectsMediaDataInRealTime property value to true so that the input accurately determines its readiness for more data. When expectsMediaDataInRealTime is true, this property value becomes false only when the input can’t process media samples at the current data rate. If this property value becomes false for a real-time source, your app may need to reduce the rate at which it appends samples, or drop them altogether.

If the canPerformMultiplePasses value of any of an asset writer’s inputs is true, the value of this property may start as false, and remain that way for extended periods.

The value of this property often changes from false to true asynchronously, as the asset writer processes and writes media samples to the output. It’s possible for this property value to temporarily be false for all inputs.

This property is key-value observable. The system doesn’t notify observers on a specific thread.

## See Also

### Appending Media Samples

var expectsMediaDataInRealTime: Bool

A Boolean value that indicates whether the input tailors its processing for real-time sources.

func requestMediaDataWhenReady(on: dispatch_queue_t, using: () -> Void)

Tells the input to request media data, at its convenience, to write to the output file.

func append(CMSampleBuffer) -> Bool

Appends a sample buffer to an input to write to the output file.

func markAsFinished()

Marks the input as finished to indicate that you’re done appending samples to it.

