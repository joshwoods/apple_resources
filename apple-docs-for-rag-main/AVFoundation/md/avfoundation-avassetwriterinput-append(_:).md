

- AVFoundation
- AVAssetWriterInput
-  append(\_:) 

Instance Method

# append(\_:)

Appends a sample buffer to an input to write to the output file.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func append(_ sampleBuffer: CMSampleBuffer) -> Bool
```

## Parameters 

`sampleBuffer`  

The sample buffer to append.

## Return Value

true if the input successfully appends the sample buffer; otherwise, false.

## Discussion

Order the samples you append according to storage requirements. For example, if you’re working with sample buffers containing compressed video, order and append them according to their decode timestamp. The system uses the timing information in the sample buffer relative to the time you set in the call to startSession(atSourceTime:) to determine the timing of samples in the output file.

If this method returns false, check the value of the asset writer’s status property to determine whether the writing operation’s status is complete, failed, or canceled. If the status is AVAssetWriter.Status.failed, the asset writer’s error property contains an error object that describes the failure.

Important

Don’t modify the sample buffer or its contents after you’ve passed it to this method.

## See Also

### Appending Media Samples

var expectsMediaDataInRealTime: Bool

A Boolean value that indicates whether the input tailors its processing for real-time sources.

var isReadyForMoreMediaData: Bool

A Boolean value that indicates whether the input is ready to accept media data.

func requestMediaDataWhenReady(on: dispatch_queue_t, using: () -> Void)

Tells the input to request media data, at its convenience, to write to the output file.

func markAsFinished()

Marks the input as finished to indicate that you’re done appending samples to it.

