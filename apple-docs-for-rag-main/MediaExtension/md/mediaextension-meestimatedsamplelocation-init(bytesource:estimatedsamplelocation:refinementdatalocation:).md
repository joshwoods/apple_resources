

- MediaExtension
- MEEstimatedSampleLocation
-  init(byteSource:estimatedSampleLocation:refinementDataLocation:) 

Initializer

# init(byteSource:estimatedSampleLocation:refinementDataLocation:)

Creates an estimated sample location object with the byte source, sample location, and data location that you specify.

macOS 14.0+

``` source
init(
    byteSource: MEByteSource,
    estimatedSampleLocation: AVSampleCursorStorageRange,
    refinementDataLocation: AVSampleCursorStorageRange
)
```

## Parameters 

`byteSource`  

The byte source to use to read the data for the sample.

`estimatedSampleLocation`  

The estimated starting file offset and size in bytes of the sample.

`refinementDataLocation`  

The starting file offset and size in bytes of the data necessary to provide an accurate sample location.

