

- Core Graphics
-  kCGPDFContextMediaBox 

Global Variable

# kCGPDFContextMediaBox

The media box for the document or for a given page.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
let kCGPDFContextMediaBox: CFString
```

## Discussion

This key is optional. If present, the value of this key must be a CFData object that contains a CGRect (stored by value, not by reference).

## See Also

### Box Keys

let kCGPDFContextCropBox: CFString

The crop box for the document or for a given page.

let kCGPDFContextBleedBox: CFString

The bleed box for the document or for a given page.

let kCGPDFContextTrimBox: CFString

The trim box for the document or for a given page.

let kCGPDFContextArtBox: CFString

The art box for the document or for a given page.

