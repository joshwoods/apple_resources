

- Vision
- VNDetectBarcodesRequest
-  coalesceCompositeSymbologies 

Instance Property

# coalesceCompositeSymbologies

A Boolean value that indicates whether to coalesce multiple codes based on the symbology.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var coalesceCompositeSymbologies: Bool { get set }
```

## See Also

### Specifying Symbologies

func supportedSymbologies() throws -> [VNBarcodeSymbology]

Returns the barcode symbologies that the request supports.

var symbologies: [VNBarcodeSymbology]

The barcode symbologies that the request detects in an image.

struct VNBarcodeSymbology

The barcode symbologies that the framework detects.

class var supportedSymbologies: [VNBarcodeSymbology]

The array of barcode symbologies that the request supports.

Deprecated

