

- AVFoundation
- AVAssetWriterInput
-  expectsMediaDataInRealTime 

Instance Property

# expectsMediaDataInRealTime

A Boolean value that indicates whether the input tailors its processing for real-time sources.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var expectsMediaDataInRealTime: Bool { get set }
```

## Discussion

Set this value to true if your app appends media data to the input from a real-time source, such as an AVCaptureOutput. Setting a true value optimizes the input for real-time usage so it accurately calculates the state of its isReadyForMoreMediaData property value.

You can’t set this value after writing starts.

Important

To ensure optimal behavior, don’t set the value of this property and performsMultiPassEncodingIfSupported to true at the same time.

## See Also

### Appending Media Samples

var isReadyForMoreMediaData: Bool

A Boolean value that indicates whether the input is ready to accept media data.

func requestMediaDataWhenReady(on: dispatch_queue_t, using: () -> Void)

Tells the input to request media data, at its convenience, to write to the output file.

func append(CMSampleBuffer) -> Bool

Appends a sample buffer to an input to write to the output file.

func markAsFinished()

Marks the input as finished to indicate that you’re done appending samples to it.

