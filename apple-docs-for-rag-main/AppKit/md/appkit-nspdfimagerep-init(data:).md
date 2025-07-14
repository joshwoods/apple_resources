

- AppKit
- NSPDFImageRep
-  init(data:) 

Initializer

# init(data:)

Returns a representation of an image initialized with the specified PDF data.

macOS

``` source
init?(data pdfData: Data)
```

## Parameters 

`pdfData`  

A data object containing the PDF data for the image.

## Return Value

An initialized NSPDFImageRep object, or `nil` if the object could not be initialized. Initialization may fail if the PDF data does not conform to the PDF file format.

## See Also

### Related Documentation

var pdfRepresentation: Data

The PDF representation of the representation’s image.

