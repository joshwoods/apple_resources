

- Vision
-  DetectBarcodesRequest 

Structure

# DetectBarcodesRequest

A request that detects barcodes in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DetectBarcodesRequest
```

## Overview

This request generates a collection of BarcodeObservation objects that describe each barcode the request detects.

## Topics

### Creating a request

init(DetectBarcodesRequest.Revision?)

Creates a barcode-detection request.

### Getting the revision

let revision: DetectBarcodesRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [DetectBarcodesRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var symbologies: [BarcodeSymbology]

The barcode symbologies that the request detects in an image.

var supportedSymbologies: [BarcodeSymbology]

The collection of barcode symbologies that the request can recognize.

enum BarcodeSymbology

The barcode symbologies that the framework detects.

var coalescesCompositeSymbologies: Bool

A Boolean value that indicates whether the request coalesces multiple codes into one.

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

struct BarcodeObservation

An object that represents barcode information that an image-analysis request detects.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

