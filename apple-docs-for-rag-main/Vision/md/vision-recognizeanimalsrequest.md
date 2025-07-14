

- Vision
-  RecognizeAnimalsRequest 

Structure

# RecognizeAnimalsRequest

A request that recognizes animals in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct RecognizeAnimalsRequest
```

## Overview

This request generates a collection of RecognizedObjectObservation objects that describe the animals the request detects.

## Topics

### Creating a request

init(RecognizeAnimalsRequest.Revision?)

Creates an animal-recognition request.

### Getting the revision

let revision: RecognizeAnimalsRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [RecognizeAnimalsRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var supportedAnimals: [RecognizeAnimalsRequest.Animal]

The collection of animals that the request can detect.

enum Animal

An identifier for a recognizable animal.

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

struct RecognizedObjectObservation

An observation with an array of classification labels that classify the recognized object.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Animal detection

struct DetectAnimalBodyPoseRequest

A request that detects an animal body pose.

