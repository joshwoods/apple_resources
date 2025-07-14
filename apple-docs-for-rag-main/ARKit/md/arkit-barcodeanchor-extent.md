

- ARKit
- BarcodeAnchor
-  extent 

Instance Property

# extent

The extent of the detected barcode’s bounds.

visionOS 2.0+

``` source
var extent: SIMD3 { get }
```

## Discussion

The width of the detected barcode is the length along the X-axis, prior to rotation about the Y-axis.

The height of the detected barcode is the length along the Z-axis, prior to rotation about the Y-axis.

## See Also

### Getting barcode information

var originFromAnchorTransform: simd_float4x4

The transform from the barcode anchor to the origin coordinate system.

var payloadData: Data

The encoded payload data of the detected barcode.

var payloadString: String?

The decoded payload string value of the detected barcode.

var symbology: BarcodeAnchor.Symbology

The symbology of the detected barcode.

enum Symbology

Values that describe specific kinds of barcodes.

var id: UUID

The unique identifier of an anchor.

