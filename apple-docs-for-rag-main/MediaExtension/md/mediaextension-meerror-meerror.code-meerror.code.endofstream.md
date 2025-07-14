

- MediaExtension
- MEError
- MEError.Code
-  MEError.Code.endOfStream 

Case

# MEError.Code.endOfStream

An error code that indicates the extension reached the end of the source file.

macOS 14.0+

``` source
case endOfStream
```

## See Also

### Error codes

case allocationFailure

An error code that indicates the extension can’t allocate memory.

case internalFailure

An error code that indicates the extension encountered an internal operation failure, such as code loading.

case invalidParameter

An error code that indicates the extension received an invalid parameter.

case locationNotAvailable

An error code that indicates specific sample isn’t contiguous, spans more than one file, or is for some other reason unsuitable for reading directly from a file.

case noSamples

An error code that indicates there are no samples in the track or a request to load a sample buffer fails.

case noSuchEdit

An error code that indicates the plug-in track reader received a request to return an edit that’s out of range.

case parsingFailure

An error code that indicates the extension encountered an error while parsing the media.

case permissionDenied

An error code that indicates the extension received a request to perform an invalid operation on a byte source.

case propertyNotSupported

An error code that indicates the extension encountered a property it doesn’t support reading and writing to.

case referenceMissing

An error code that indicates the decoder received a request to decode a sample without decoding the required reference frame dependencies first.

case unsupportedFeature

An error code that indicates the extension doesn’t support an aspect of the media.

