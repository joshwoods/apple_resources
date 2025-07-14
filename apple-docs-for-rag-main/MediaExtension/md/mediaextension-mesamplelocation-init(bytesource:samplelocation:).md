

- MediaExtension
- MESampleLocation
-  init(byteSource:sampleLocation:) 

Initializer

# init(byteSource:sampleLocation:)

Creates a sample location object with the byte source and sample location that you specify.

macOS 14.0+

``` source
init(
    byteSource: MEByteSource,
    sampleLocation: AVSampleCursorStorageRange
)
```

## Parameters 

`byteSource`  

The byte source to use to read the data for the sample.

`sampleLocation`  

The starting file offset and size in bytes of the sample.

