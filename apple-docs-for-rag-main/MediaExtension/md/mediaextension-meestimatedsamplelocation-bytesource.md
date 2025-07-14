

- MediaExtension
- MEEstimatedSampleLocation
-  byteSource 

Instance Property

# byteSource

The byte source to use to read the data for the sample.

macOS 14.0+

``` source
var byteSource: MEByteSource { get }
```

## See Also

### Inspecting an estimated sample location

var estimatedSampleLocation: AVSampleCursorStorageRange

The estimated starting file offset and size in bytes of the sample.

var refinementDataLocation: AVSampleCursorStorageRange

The starting file offset and size in bytes of the data necessary to provide an accurate sample location.

