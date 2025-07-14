

- AppKit
- NSPICTImageRep
-  init(data:) 

Initializer

# init(data:)

Returns a representation of an image from the specified data in the PICT file format.

macOS

``` source
init?(data pictData: Data)
```

## Parameters 

`pictData`  

A data object containing the PICT data.

## Return Value

An initialized NSPICTImageRep, or `nil` if the object could not be initialized. Initialization may fail if the data does not conform to the PICT file format.

## Discussion

If the PICT data is obtained directly from a PICT file or document, this method ignores most of the 512-byte header that occurs before the start of the actual picture data. It may retrieve some relevant meta information from the header.

## See Also

### Related Documentation

var pictRepresentation: Data

The image representation’s PICT data.

