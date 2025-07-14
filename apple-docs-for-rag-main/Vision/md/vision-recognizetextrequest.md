

- Vision
-  RecognizeTextRequest 

Structure

# RecognizeTextRequest

An image-analysis request that recognizes text in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct RecognizeTextRequest
```

## Overview

This request generates a collection of RecognizedTextObservation objects that describe the text the request detects. By default, a text-recognition request first locates all possible glyphs or characters in the input image, and then analyzes each string. To specify or limit the languages to find in the request, set recognitionLanguages to an array that contains the names of the languages of text you want to recognize.

## Topics

### Creating a request

init(RecognizeTextRequest.Revision?)

Creates a text-recognition request.

### Getting the revision

let revision: RecognizeTextRequest.Revision

The algorithm or implementation the request uses.

static let supportedRevisions: [RecognizeTextRequest.Revision]

The collection of revisions the request supports.

enum Revision

A type that describes the algorithm or implementation that the request performs.

### Inspecting a request

var automaticallyDetectsLanguage: Bool

A Boolean value that indicates whether to attempt detecting the language to use the appropriate model for recognition and language correction.

var usesLanguageCorrection: Bool

A Boolean value that indicates whether the request applies language correction during the recognition process.

var supportedRecognitionLanguages: [Locale.Language]

The identifiers of the languages that the request supports.

var customWords: [String]

An array of strings to supplement the recognized languages at the word-recognition stage.

var minimumTextHeightFraction: Float

The minimum height, relative to the image height, of the text to recognize.

var recognitionLanguages: [Locale.Language]

An array of languages to detect, in priority order.

var recognitionLevel: RecognizeTextRequest.RecognitionLevel

A value that determines whether the request prioritizes accuracy or speed in text recognition.

enum RecognitionLevel

Constants that identify the performance and accuracy of the text recognition.

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

struct RecognizedTextObservation

An object that contains information about both the location and content of text and glyphs that the framework recognizes in an image.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- ImageProcessingRequest
- Sendable
- VisionRequest

## See Also

### Text detection

Locating and displaying recognized text

Perform text recognition on a photo using the Vision framework’s text-recognition request.

struct DetectTextRectanglesRequest

An image-analysis request that finds regions of visible text in an image.

