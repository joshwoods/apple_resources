

- MediaExtension
- MEEstimatedSampleLocation
-  estimatedSampleLocation 

Instance Property

# estimatedSampleLocation

The estimated starting file offset and size in bytes of the sample.

macOS 14.0+

``` source
var estimatedSampleLocation: AVSampleCursorStorageRange { get }
```

## See Also

### Inspecting an estimated sample location

var byteSource: MEByteSource

The byte source to use to read the data for the sample.

var refinementDataLocation: AVSampleCursorStorageRange

The starting file offset and size in bytes of the data necessary to provide an accurate sample location.

