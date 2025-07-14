

- ARKit
- BarcodeAnchor
-  symbology 

Instance Property

# symbology

The symbology of the detected barcode.

visionOS 2.0+

``` source
var symbology: BarcodeAnchor.Symbology { get }
```

## See Also

### Getting barcode information

var extent: SIMD3&lt;Float>

The extent of the detected barcode’s bounds.

var originFromAnchorTransform: simd_float4x4

The transform from the barcode anchor to the origin coordinate system.

var payloadData: Data

The encoded payload data of the detected barcode.

var payloadString: String?

The decoded payload string value of the detected barcode.

enum Symbology

Values that describe specific kinds of barcodes.

var id: UUID

The unique identifier of an anchor.

