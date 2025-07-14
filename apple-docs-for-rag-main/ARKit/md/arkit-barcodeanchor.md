

- ARKit
-  BarcodeAnchor 

Structure

# BarcodeAnchor

A barcode’s position in a person’s surroundings.

visionOS 2.0+

``` source
struct BarcodeAnchor
```

## Overview

A `BarcodeAnchor` describes a barcode that ARKit detects in a person’s surroundings. A barcode anchor has exactly one BarcodeSymbology that indicates which type of barcode the framework detects. It also includes properties, such as the barcode’s payload data, which is a decoded string value of that data.

## Topics

### Getting barcode information

var extent: SIMD3&lt;Float>

The extent of the detected barcode’s bounds.

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

### Instance Properties

var description: String

A textual representation of this anchor.

## Relationships

### Conforms To

- Anchor
- CustomStringConvertible
- Identifiable
- Sendable

## See Also

### Barcode detection

class BarcodeDetectionProvider

An object that provides the real-time position of barcodes the framework detects in a person’s environment.

