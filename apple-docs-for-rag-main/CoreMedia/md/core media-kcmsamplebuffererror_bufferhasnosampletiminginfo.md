

- Core Media
-  kCMSampleBufferError_BufferHasNoSampleTimingInfo 

Global Variable

# kCMSampleBufferError_BufferHasNoSampleTimingInfo

An error code that indicates a request for sample timing on a buffer failed because the buffer doesn’t contain that information.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCMSampleBufferError_BufferHasNoSampleTimingInfo: OSStatus { get }
```

## See Also

### Error Codes

var kCMSampleBufferError_AllocationFailed: OSStatus

An error code that indicates the system failed to allocate memory.

var kCMSampleBufferError_AlreadyHasDataBuffer: OSStatus

An error code that indicates an attempt to set data on a sample buffer failed because that buffer already contains media data.

var kCMSampleBufferError_ArrayTooSmall: OSStatus

An error code that indicates the output array isn’t large enough to hold the requested array.

var kCMSampleBufferError_BufferHasNoSampleSizes: OSStatus

An error code that indicates a request for sample sizes on a buffer failed because the buffer doesn’t provide that information.

var kCMSampleBufferError_BufferNotReady: OSStatus

An error code that indicates the system can’t make the buffer’s data ready for use.

var kCMSampleBufferError_CannotSubdivide: OSStatus

An error code that indicates a sample buffer doesn’t contain sample sizes.

var kCMSampleBufferError_DataCanceled: OSStatus

An error code that indicates a sample buffer canceled its data-loading operation.

var kCMSampleBufferError_DataFailed: OSStatus

An error code that indicates a sample buffer failed to load its data.

var kCMSampleBufferError_InvalidEntryCount: OSStatus

An error code that indicates a timing or size value isn’t within the allowed range.

var kCMSampleBufferError_InvalidMediaFormat: OSStatus

An error code that indicates the media format doesn’t match the sample buffer’s format description.

var kCMSampleBufferError_InvalidMediaTypeForOperation: OSStatus

An error code that indicates the media type that the format description defines isn’t a value for the requested operation.

var kCMSampleBufferError_InvalidSampleData: OSStatus

An error code that indicates the sample buffer contains bad data.

var kCMSampleBufferError_Invalidated: OSStatus

An error code that indicates a sample buffer invalidated its data.

var kCMSampleBufferError_RequiredParameterMissing: OSStatus

An error code that indicates a required parameter’s value is invalid.

var kCMSampleBufferError_SampleIndexOutOfRange: OSStatus

An error code that indicates the sample index is outside the range of samples that the buffer contains.

