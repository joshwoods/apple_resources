

- Core Media
-  CMSampleBufferCallBlockForEachSample(\_:\_:) 

Function

# CMSampleBufferCallBlockForEachSample(\_:\_:)

Calls a block for every individual sample in a sample buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferCallBlockForEachSample(
    _ sbuf: CMSampleBuffer,
    _ handler: (CMSampleBuffer, CMItemCount) -> OSStatus
) -> OSStatus
```

## Parameters 

`sbuf`  

`CMSampleBuffer` that may contain multiple samples.

`handler`  

Block to be called for each individual sample.

## Discussion

Temporary sample buffers will be created for individual samples, referring to the sample data and containing its timing, size and attachments. The block may retain these sample buffers if desired. If the block returns an error, iteration will stop immediately and the error will be returned.

If there are no sample sizes in the provided sample buffer, `kCMSampleBufferError_CannotSubdivide` will be returned. This will happen, for example, if the samples in the buffer are non-contiguous (for example, non-interleaved audio, where the channel values for a single sample are scattered through the buffer).

## See Also

### Processing Samples

func CMSampleBufferCallForEachSample(CMSampleBuffer, callback: (CMSampleBuffer, CMItemCount, UnsafeMutableRawPointer?) -> OSStatus, refcon: UnsafeMutableRawPointer?) -> OSStatus

Calls a function for every individual sample in a sample buffer.

