

- AppKit
- NSPICTImageRep
-  boundingBox 

Instance Property

# boundingBox

The rectangle that bounds the image representation.

macOS

``` source
var boundingBox: NSRect { get }
```

## Discussion

The rectangle bounding the receiver. This rectangle is obtained from the the `picFrame` field in the picture header. See the Carbon QuickDraw Manager documentation for information on the picture header

## See Also

### Getting Data

var pictRepresentation: Data

The image representation’s PICT data.

