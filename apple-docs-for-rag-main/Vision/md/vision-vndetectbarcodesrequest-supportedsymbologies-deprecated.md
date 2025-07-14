

- Vision
- VNDetectBarcodesRequest
-  supportedSymbologies Deprecated

Type Property

# supportedSymbologies

The array of barcode symbologies that the request supports.

iOS 11.0–15.0DeprecatediPadOS 11.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.13–12.0DeprecatedtvOS 11.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class var supportedSymbologies: [VNBarcodeSymbology] { get }
```

Deprecated

Use supportedSymbologies() instead.

## Discussion

Calling this method can be an expensive operation.

## See Also

### Specifying Symbologies

func supportedSymbologies() throws -> [VNBarcodeSymbology]

Returns the barcode symbologies that the request supports.

var symbologies: [VNBarcodeSymbology]

The barcode symbologies that the request detects in an image.

var coalesceCompositeSymbologies: Bool

A Boolean value that indicates whether to coalesce multiple codes based on the symbology.

struct VNBarcodeSymbology

The barcode symbologies that the framework detects.

