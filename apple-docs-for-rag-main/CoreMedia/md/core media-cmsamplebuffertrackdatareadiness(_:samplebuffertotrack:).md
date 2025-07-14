

- Core Media
-  CMSampleBufferTrackDataReadiness(\_:sampleBufferToTrack:) 

Function

# CMSampleBufferTrackDataReadiness(\_:sampleBufferToTrack:)

Associates a sample buffer’s data readiness with that of another sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferTrackDataReadiness(
    _ sbuf: CMSampleBuffer,
    sampleBufferToTrack: CMSampleBuffer
) -> OSStatus
```

## Parameters 

`sbuf`  

The sample buffer being modified.

`sampleBufferToTrack`  

The sample buffer being tracked.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

After calling this API, if `CMSampleBufferDataIsReady` is called, it will return `sampleBufferToTrack`’s data readiness. If `CMSampleBufferMakeDataReady` is called, it will make `sampleBufferToTrack` data ready.

Example of use: This allows bursting a multi-sample `CMSampleBuffer` into single-sample `CMSampleBuffers` before the data is ready. The single-sample `CMSampleBuffers` will all track the multi-sample `CMSampleBuffer’s` data readiness.

## See Also

### Determining Readiness

func CMSampleBufferDataIsReady(CMSampleBuffer) -> Bool

Returns a Boolean value that indicates whether the sample buffer’s data is ready for use.

func CMSampleBufferSetDataReady(CMSampleBuffer) -> OSStatus

Marks a sample buffer’s data as ready for use.

func CMSampleBufferSetDataFailed(CMSampleBuffer, status: OSStatus) -> OSStatus

Marks the sample buffer’s data as failed to indicate that it won’t become ready.

func CMSampleBufferHasDataFailed(CMSampleBuffer, statusOut: UnsafeMutablePointer&lt;OSStatus>?) -> Bool

Returns a Boolean value that indicates whether the sample buffer’s data loading request failed.

func CMSampleBufferMakeDataReady(CMSampleBuffer) -> OSStatus

Makes the sample buffer’s data ready for use by invoking its callback to load the data.

