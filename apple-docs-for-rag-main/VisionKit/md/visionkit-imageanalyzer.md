

- VisionKit
-  ImageAnalyzer 

Class

# ImageAnalyzer

An object that finds items in images that people can interact with, such as subjects, text, and QR codes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
final class ImageAnalyzer
```

## Mentioned in 

Enabling Live Text interactions with images

## Overview

To use an `ImageAnalyzer` object, first create an ImageAnalyzer.Configuration object, and specify the types of items you want to find in an image. Then pass the image you want to analyze and the configuration object to an `ImageAnalyzer` object using the analyze(_:configuration:) or similar method. This method returns an ImageAnalysis object that contains all the data VisionKit needs to implement the Live Text interface.

Next, show the Live Text interface. For iOS apps, set the interaction object of the view that contains the image to an instance of ImageAnalysisInteraction and set its analysis property to the `ImageAnalysis` object. To enable interactions with the image, set the interaction object’s preferredInteractionTypes property. To customize the Live Text interface, set the `ImageAnalysisInteraction `object’s delegate property and implement the ImageAnalysisInteractionDelegate protocol methods.

For macOS apps, add an `ImageAnalysisOverlayView` object above the view that contains the image, and set its `analysis` property. To enable interactions with the image, set the overlay view’s `preferredInteractionTypes` property. Set the `ImageAnalysisOverlayView `object’s `delegate` property and implement the `ImageAnalysisOverlayViewDelegate` protocol methods.

By default, the Live Text interface starts immediately when you show the view.

## Topics

### Handling availability

class var isSupported: Bool

A Boolean value that indicates whether the device supports image analysis.

class var supportedTextRecognitionLanguages: [String]

The identifiers for the languages that the image analyzer recognizes.

### Creating image analyzers

init()

Creates an image analyzer that identifies subjects, text, and machine-readable codes in images.

### Configuring image analyzers

struct Configuration

A configuration that specifies the types of items and locales that the image analyzer recognizes.

### Finding items in images

func analyze(UIImage, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with an image.

func analyze(NSImage, orientation: CGImagePropertyOrientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with an image in the specified orientation.

func analyze(CGImage, orientation: CGImagePropertyOrientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with a Core Graphics image in the specified orientation.

func analyze(CVPixelBuffer, orientation: CGImagePropertyOrientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with a pixel buffer image in the specified orientation.

func analyze(CIImage, orientation: CGImagePropertyOrientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with a bitmap image in the specified orientation.

func analyze(UIImage, orientation: UIImage.Orientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with an image in the specified orientation.

func analyze(imageAt: URL, orientation: CGImagePropertyOrientation, configuration: ImageAnalyzer.Configuration) async throws -> ImageAnalysis

Returns the data for providing a Live Text interaction with an image at a URL and in the specified orientation.

### Structures

struct AnalysisTypes

The types of items that an image analyzer looks for in an image.

## Relationships

### Conforms To

- Sendable

## See Also

### Content recognition and interaction in images

Enabling Live Text interactions with images

Add a Live Text interface that enables users to perform actions with text and QR codes that appear in images.

class ImageAnalysis

An object that represents the results of analyzing an image, and provides the input for the Live Text interface object.

class ImageAnalysisInteraction

An interface that enables people to interact with recognized text, barcodes, and other objects in an image.

protocol ImageAnalysisInteractionDelegate

A delegate that handles image-analysis and user-interaction callbacks for an interaction object.

class ImageAnalysisOverlayView

A view that enables people to interact with recognized text, barcodes, and other objects in an image.

protocol ImageAnalysisOverlayViewDelegate

A delegate that handles image-analysis and user-interaction callbacks for an overlay view.

