

- Core Media
- CMSampleBuffer
- CMSampleBuffer.Error
-  dataCanceled 

Type Property

# dataCanceled

A sample buffer canceled its data loading operation.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let dataCanceled: NSError
```

## See Also

### Errors

static let allocationFailed: NSError

The system failed to allocate memory.

static let alreadyHasDataBuffer: NSError

You attempted to set data on a sample buffer that already contains media data.

static let arrayTooSmall: NSError

The output array isn’t large enough to hold the requested array.

static let bufferHasNoSampleSizes: NSError

You requested sample sizes on a buffer that doesn’t provide that information.

static let bufferHasNoSampleTimingInfo: NSError

You requested sample timing on a buffer that doesn’t contain that information.

static let bufferNotReady: NSError

The system can’t make the buffer’s data ready for use.

static let cannotSubdivide: NSError

A sample buffer doesn’t contain sample sizes.

static let dataFailed: NSError

A sample buffer failed to load its data.

static let invalidEntryCount: NSError

A timing or size value isn’t within the allowed range.

static let invalidMediaFormat: NSError

The format of the media doesn’t match the sample buffer’s format description.

static let invalidMediaTypeForOperation: NSError

The media type the format description defines isn’t value for the requested operation.

static let invalidSampleData: NSError

The sample buffer contains bad data.

static let invalidated: NSError

A sample buffer invalidated its data.

static let requiredParameterMissing: NSError

You didn’t provide a valid value for a required parameter.

static let sampleIndexOutOfRange: NSError

You specified a sample index that’s outside of the range of samples that the buffer contains.

