

- Core Media
-  CMSampleBufferSetDataFailed(\_:status:) 

Function

# CMSampleBufferSetDataFailed(\_:status:)

Marks the sample buffer’s data as failed to indicate that it won’t become ready.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferSetDataFailed(
    _ sbuf: CMSampleBuffer,
    status: OSStatus
) -> OSStatus
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being modified.

`status`  

A status describing the failure.

## See Also

### Determining Readiness

func CMSampleBufferDataIsReady(CMSampleBuffer) -> Bool

Returns a Boolean value that indicates whether the sample buffer’s data is ready for use.

func CMSampleBufferSetDataReady(CMSampleBuffer) -> OSStatus

Marks a sample buffer’s data as ready for use.

func CMSampleBufferHasDataFailed(CMSampleBuffer, statusOut: UnsafeMutablePointer&lt;OSStatus>?) -> Bool

Returns a Boolean value that indicates whether the sample buffer’s data loading request failed.

func CMSampleBufferMakeDataReady(CMSampleBuffer) -> OSStatus

Makes the sample buffer’s data ready for use by invoking its callback to load the data.

func CMSampleBufferTrackDataReadiness(CMSampleBuffer, sampleBufferToTrack: CMSampleBuffer) -> OSStatus

Associates a sample buffer’s data readiness with that of another sample buffer.

