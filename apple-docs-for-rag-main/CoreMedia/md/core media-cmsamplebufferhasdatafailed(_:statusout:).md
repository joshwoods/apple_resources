

- Core Media
-  CMSampleBufferHasDataFailed(\_:statusOut:) 

Function

# CMSampleBufferHasDataFailed(\_:statusOut:)

Returns a Boolean value that indicates whether the sample buffer’s data loading request failed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferHasDataFailed(
    _ sbuf: CMSampleBuffer,
    statusOut: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

`statusOut`  

Points to an `OSStatus` to receive a status code describing the failure. Pass `NULL` if you don’t want this information.

## See Also

### Determining Readiness

func CMSampleBufferDataIsReady(CMSampleBuffer) -> Bool

Returns a Boolean value that indicates whether the sample buffer’s data is ready for use.

func CMSampleBufferSetDataReady(CMSampleBuffer) -> OSStatus

Marks a sample buffer’s data as ready for use.

func CMSampleBufferSetDataFailed(CMSampleBuffer, status: OSStatus) -> OSStatus

Marks the sample buffer’s data as failed to indicate that it won’t become ready.

func CMSampleBufferMakeDataReady(CMSampleBuffer) -> OSStatus

Makes the sample buffer’s data ready for use by invoking its callback to load the data.

func CMSampleBufferTrackDataReadiness(CMSampleBuffer, sampleBufferToTrack: CMSampleBuffer) -> OSStatus

Associates a sample buffer’s data readiness with that of another sample buffer.

