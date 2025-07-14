

- Vision
- VNDetectBarcodesRequest
-  symbologies 

Instance Property

# symbologies

The barcode symbologies that the request detects in an image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var symbologies: [VNBarcodeSymbology] { get set }
```

## Discussion

By default, a request scans for all symbologies. Specify a subset of symbologies to limit the request’s detection range.

Note

Setting a revision on the request resets the symbologies to all symbologies for the specified revision.

## See Also

### Specifying Symbologies

func supportedSymbologies() throws -> [VNBarcodeSymbology]

Returns the barcode symbologies that the request supports.

var coalesceCompositeSymbologies: Bool

A Boolean value that indicates whether to coalesce multiple codes based on the symbology.

struct VNBarcodeSymbology

The barcode symbologies that the framework detects.

class var supportedSymbologies: [VNBarcodeSymbology]

The array of barcode symbologies that the request supports.

Deprecated

