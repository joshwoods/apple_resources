

- Vision
-  ClassifyImageRequest 

Structure

# ClassifyImageRequest

A request to classify an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct ClassifyImageRequest
```

## Overview

This type of request produces a collection of ClassificationObservation objects that describe an image. Access the possible classifications through the supportedIdentifiers property.

```
if let imageURL = Bundle.main.url(forResource: "ClassificationImage",
                                      withExtension: "jpg") {
    do {
        let request = ClassifyImageRequest()
        let results = try await request.perform(on: imageURL)
        for classification in results {
            print("Classified \(classification.identifier)")
        }
    } catch {
        print("Encountered an error when performing the request: \(error.localizedDescription)")
    }
}
```

## Topics

### Creating a request

init(ClassifyImageRequest.Revision?)

Creates an image-classifier request.

### Getting the revision

let revision: ClassifyImageRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [ClassifyImageRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var cropAndScaleAction: ImageCropAndScaleAction

An optional setting that tells the algorithm how to scale an input image before generating the result.

enum ImageCropAndScaleAction

A scale to apply to an input image before performing a request.

var supportedIdentifiers: [String]

The classification identifiers the request supports.

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

struct ClassificationObservation

An object that represents classification information that an image-analysis request produces.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Still-image analysis

Classifying images for categorization and search

Analyze and label images using a Vision classification request.

protocol ImageProcessingRequest

A type for image-analysis requests that focus on a specific part of an image.

class ImageRequestHandler

An object that processes one or more image-analysis requests pertaining to a single image.

protocol VisionRequest

A type for image-analysis requests.

protocol VisionObservation

A type for objects produced by image-analysis requests.

