

- MediaExtension
- MEError
-  noSuchEdit 

Type Property

# noSuchEdit

An error code that indicates the plug-in track reader received a request to return an edit that’s out of range.

macOS 14.0+

``` source
static var noSuchEdit: MEError.Code { get }
```

## See Also

### Identifying the error domain and codes

static var errorDomain: String

The domain of the error.

static var allocationFailure: MEError.Code

An error code that indicates the extension can’t allocate memory.

static var endOfStream: MEError.Code

An error code that indicates the extension reached the end of the source file.

static var internalFailure: MEError.Code

An error code that indicates the extension encountered an internal operation failure, such as code loading.

static var invalidParameter: MEError.Code

An error code that indicates the extension received an invalid parameter.

static var locationNotAvailable: MEError.Code

An error code that indicates a specific sample isn’t contiguous, spans more than one file, or is for some other reason unsuitable to read directly from a file.

static var noSamples: MEError.Code

An error code that indicates there are no samples in the track or a request to load a sample buffer fails.

static var parsingFailure: MEError.Code

An error code that indicates the extension encountered an error while parsing the media.

static var permissionDenied: MEError.Code

An error code that indicates the extension received a request to perform an invalid operation on a byte source.

static var propertyNotSupported: MEError.Code

An error code that indicates the extension encountered a property it doesn’t support reading and writing to.

static var referenceMissing: MEError.Code

An error code that indicates the decoder received a request to decode a sample without decoding the required reference frame dependencies first.

static var unsupportedFeature: MEError.Code

An error code that indicates the extension doesn’t support an aspect of the media.

