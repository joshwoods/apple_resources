

- Core Media
-  CMSampleBufferMakeDataReady(\_:) 

Function

# CMSampleBufferMakeDataReady(\_:)

Makes the sample buffer’s data ready for use by invoking its callback to load the data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferMakeDataReady(_ sbuf: CMSampleBuffer) -> OSStatus
```

## Parameters 

`sbuf`  

The sample buffer being modified.

## Return Value

A result code. See Sample Buffer Error Codes.

## Discussion

The `CMSampleBufferMakeDataReadyCallback` is passed in by the client during creation. It must return 0 if successful, and in that case, `CMSampleBufferMakeDataReady` sets the data readiness of the `CMSampleBuffer` to true. If the sample buffer isn’t ready, and there’s no `CMSampleBufferMakeDataReadyCallback` to call, `kCMSampleBufferError_BufferNotReady` will be returned. Similarly, if the `CMSampleBuffer` isn’t ready, and the `CMSampleBufferMakeDataReadyCallback` fails and returns an error, CMSampleBuffer will be returned.

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

func CMSampleBufferTrackDataReadiness(CMSampleBuffer, sampleBufferToTrack: CMSampleBuffer) -> OSStatus

Associates a sample buffer’s data readiness with that of another sample buffer.

