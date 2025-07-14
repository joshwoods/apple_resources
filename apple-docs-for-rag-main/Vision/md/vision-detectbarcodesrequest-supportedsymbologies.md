

- Vision
- DetectBarcodesRequest
-  supportedSymbologies 

Instance Property

# supportedSymbologies

The collection of barcode symbologies that the request can recognize.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var supportedSymbologies: [BarcodeSymbology] { get }
```

## Discussion

Using this property could be a potentially expensive operation.

## See Also

### Inspecting a request

var symbologies: [BarcodeSymbology]

The barcode symbologies that the request detects in an image.

enum BarcodeSymbology

The barcode symbologies that the framework detects.

var coalescesCompositeSymbologies: Bool

A Boolean value that indicates whether the request coalesces multiple codes into one.

