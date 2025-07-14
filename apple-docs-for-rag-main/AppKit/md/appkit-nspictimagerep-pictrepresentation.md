

- AppKit
- NSPICTImageRep
-  pictRepresentation 

Instance Property

# pictRepresentation

The image representation’s PICT data.

macOS

``` source
var pictRepresentation: Data { get }
```

## Discussion

The data does not include the 512-byte header, if it was present in the original data. If you want to write the data to a file, you must precede it with a 512-byte header (containing all zeros) if you want to conform to the PICT document format.

## See Also

### Getting Data

var boundingBox: NSRect

The rectangle that bounds the image representation.

