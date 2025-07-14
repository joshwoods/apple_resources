

- Vision
- VNDetectBarcodesRequest
-  supportedSymbologies() 

Instance Method

# supportedSymbologies()

Returns the barcode symbologies that the request supports.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func supportedSymbologies() throws -> [VNBarcodeSymbology]
```

## Return Value

An array of symbologies.

## See Also

### Specifying Symbologies

var symbologies: [VNBarcodeSymbology]

The barcode symbologies that the request detects in an image.

var coalesceCompositeSymbologies: Bool

A Boolean value that indicates whether to coalesce multiple codes based on the symbology.

struct VNBarcodeSymbology

The barcode symbologies that the framework detects.

class var supportedSymbologies: [VNBarcodeSymbology]

The array of barcode symbologies that the request supports.

Deprecated

