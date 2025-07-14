

- Vision
- DetectBarcodesRequest
-  symbologies 

Instance Property

# symbologies

The barcode symbologies that the request detects in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var symbologies: [BarcodeSymbology]
```

## Discussion

By default, a request scans for all symbologies. Specify a subset of symbologies to limit the request’s detection range.

## See Also

### Inspecting a request

var supportedSymbologies: [BarcodeSymbology]

The collection of barcode symbologies that the request can recognize.

enum BarcodeSymbology

The barcode symbologies that the framework detects.

var coalescesCompositeSymbologies: Bool

A Boolean value that indicates whether the request coalesces multiple codes into one.

