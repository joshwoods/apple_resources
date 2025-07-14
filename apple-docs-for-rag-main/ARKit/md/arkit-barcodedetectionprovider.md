

- ARKit
-  BarcodeDetectionProvider 

Class

# BarcodeDetectionProvider

An object that provides the real-time position of barcodes the framework detects in a person’s environment.

visionOS 2.0+

``` source
final class BarcodeDetectionProvider
```

## Overview

Use this provider to receive updates about barcodes that ARKit detect in a person’s surroundings, This provider returns the results in the form of an asynchronous sequence of BarcodeAnchor structures. Your app needs to include the Spatial barcode and QR code scanning entitlement to use this capability; otherwise, it has no effect.

## Topics

### Creating a barcode detection provider

init(symbologies: [BarcodeAnchor.Symbology])

Creates a barcode detection provider that looks for the specified symbologies.

### Inspecting a barcode detection provider

var anchorUpdates: AnchorUpdateSequence&lt;BarcodeAnchor>

An asynchronous sequence of anchor updates that describe the anchors in a person’s surroundings.

var description: String

A textual representation of this barcode detection provider.

var state: DataProviderState

The state of a barcode detection provider.

### Type properties

static var isSupported: Bool

A Boolean value that determines whether a device supports the barcode detection provider.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The authorization types you need to use the barcode detection provider.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

## See Also

### Barcode detection

struct BarcodeAnchor

A barcode’s position in a person’s surroundings.

