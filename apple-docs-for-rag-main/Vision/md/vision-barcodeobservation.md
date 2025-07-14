

- Vision
-  BarcodeObservation 

Structure

# BarcodeObservation

An object that represents barcode information that an image-analysis request detects.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct BarcodeObservation
```

## Topics

### Creating an observation

init(VNBarcodeObservation)

Creates a barcode observation.

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let isColorInverted: Bool

A Boolean value that indicates whether the barcode is color inverted.

let isGS1DataCarrier: Bool

A Boolean value that indicates whether the barcode carries any global standards data.

### Getting the payload

let payloadData: Data?

The raw data representation of the barcode’s payload.

let payloadString: String?

A string value that represents the barcode payload.

let supplementalPayloadData: Data?

The raw data representation of the barcode’s supplemental payload.

let supplementalPayloadString: String?

The supplemental code decoded as a string value.

### Getting the symbology

let symbology: BarcodeSymbology

The symbology of the observed barcode.

enum BarcodeSymbology

The barcode symbologies that the framework detects.

### Getting the composite type

let supplementalCompositeType: BarcodeObservation.CompositeType?

The supplemental composite type.

enum CompositeType

Composite types for barcode requests.

## Relationships

### Conforms To

- BoundingBoxProviding
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- QuadrilateralProviding
- Sendable
- VisionObservation

## See Also

### Performing a request

func perform(on: URL, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on an image URL and produces observations.

**Required** Default implementations provided.

func perform(on: Data, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on image data and produces observations.

**Required** Default implementations provided.

func perform(on: CGImage, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Graphics image and produces observations.

**Required** Default implementations provided.

func perform(on: CVPixelBuffer, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a pixel buffer and produces observations.

**Required** Default implementations provided.

func perform(on: CMSampleBuffer, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Media buffer and produces observations.

**Required** Default implementations provided.

func perform(on: CIImage, orientation: CGImagePropertyOrientation?) async throws -> Self.Result

Performs the request on a Core Image image and produces observations.

**Required** Default implementations provided.

