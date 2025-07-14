

- MediaExtension
- MEEstimatedSampleLocation
-  refinementDataLocation 

Instance Property

# refinementDataLocation

The starting file offset and size in bytes of the data necessary to provide an accurate sample location.

macOS 14.0+

``` source
var refinementDataLocation: AVSampleCursorStorageRange { get }
```

## Discussion

Pass this refinement data to the refineSampleLocation(_:refinementData:refinementDataLength:refinedLocation:) to determine the exact sample location.

## See Also

### Inspecting an estimated sample location

var byteSource: MEByteSource

The byte source to use to read the data for the sample.

var estimatedSampleLocation: AVSampleCursorStorageRange

The estimated starting file offset and size in bytes of the sample.

