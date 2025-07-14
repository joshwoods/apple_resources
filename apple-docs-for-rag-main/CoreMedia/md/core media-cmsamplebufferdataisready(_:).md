

- Core Media
-  CMSampleBufferDataIsReady(\_:) 

Function

# CMSampleBufferDataIsReady(\_:)

Returns a Boolean value that indicates whether the sample buffer’s data is ready for use.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferDataIsReady(_ sbuf: CMSampleBuffer) -> Bool
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

## Return Value

A Boolean indicating whether or not the sample buffer’s data is ready. True is returned for special marker buffers, even though they have no data. False is returned if there is an error.

## See Also

### Determining Readiness

func CMSampleBufferSetDataReady(CMSampleBuffer) -> OSStatus

Marks a sample buffer’s data as ready for use.

func CMSampleBufferSetDataFailed(CMSampleBuffer, status: OSStatus) -> OSStatus

Marks the sample buffer’s data as failed to indicate that it won’t become ready.

func CMSampleBufferHasDataFailed(CMSampleBuffer, statusOut: UnsafeMutablePointer&lt;OSStatus>?) -> Bool

Returns a Boolean value that indicates whether the sample buffer’s data loading request failed.

func CMSampleBufferMakeDataReady(CMSampleBuffer) -> OSStatus

Makes the sample buffer’s data ready for use by invoking its callback to load the data.

func CMSampleBufferTrackDataReadiness(CMSampleBuffer, sampleBufferToTrack: CMSampleBuffer) -> OSStatus

Associates a sample buffer’s data readiness with that of another sample buffer.

