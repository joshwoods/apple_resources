

- Core Media
-  CMSampleBufferCallForEachSample(\_:callback:refcon:) 

Function

# CMSampleBufferCallForEachSample(\_:callback:refcon:)

Calls a function for every individual sample in a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferCallForEachSample(
    _ sbuf: CMSampleBuffer,
    callback: (CMSampleBuffer, CMItemCount, UnsafeMutableRawPointer?) -> OSStatus,
    refcon: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`sbuf`  

The sample buffer that may contain multiple samples.

`callback`  

Function to be called for each individual sample.

`refcon`  

Refcon to be passed to the callback function.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

The system will create temporary sample buffers for individual samples. Each sample buffer will refer to the sample data and contain its timing, size, and attachments.

The callback function may retain these sample buffers if desired. If the callback function returns an error, iteration will stop immediately and function returns the error received from the callback. The function will return `kCMSampleBufferError_CannotSubdivide` error if there are no sample sizes in the provided sample buffer. This will happen, for example, if the samples in the buffer are non-contiguous (for example, non-interleaved audio, where the channel values for a single sample are scattered through the buffer).

## See Also

### Processing Samples

func CMSampleBufferCallBlockForEachSample(CMSampleBuffer, (CMSampleBuffer, CMItemCount) -> OSStatus) -> OSStatus

Calls a block for every individual sample in a sample buffer.

