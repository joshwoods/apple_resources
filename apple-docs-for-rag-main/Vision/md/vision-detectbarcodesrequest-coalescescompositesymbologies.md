

- Vision
- DetectBarcodesRequest
-  coalescesCompositeSymbologies 

Instance Property

# coalescesCompositeSymbologies

A Boolean value that indicates whether the request coalesces multiple codes into one.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var coalescesCompositeSymbologies: Bool
```

## Discussion

The default value for this property is `false`.

## See Also

### Inspecting a request

var symbologies: [BarcodeSymbology]

The barcode symbologies that the request detects in an image.

var supportedSymbologies: [BarcodeSymbology]

The collection of barcode symbologies that the request can recognize.

enum BarcodeSymbology

The barcode symbologies that the framework detects.

