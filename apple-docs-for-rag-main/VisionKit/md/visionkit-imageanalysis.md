

- VisionKit
-  ImageAnalysis 

Class

# ImageAnalysis

An object that represents the results of analyzing an image, and provides the input for the Live Text interface object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
final class ImageAnalysis
```

## Overview

An `ImageAnalysis` object represents the results of an ImageAnalyzer object finding items in an image that people can interact with. To create an `ImageAnalysis` object, use the `ImageAnalyzer` class’s analyze(_:configuration:) method variety, passing the image and an ImageAnalyzer.Configuration object that specifies the items you want to find. Then pass the image analysis to either an ImageAnalysisInteraction object for iOS or an ImageAnalysisOverlayView object for macOS to provide the Live Text interface.

## Topics

### Checking results

func hasResults(for: ImageAnalyzer.AnalysisTypes) -> Bool

Returns a Boolean value that indicates whether the analysis finds the specified types in the image.

### Getting the text

var transcript: String

The string that the text items in the image represent.

## See Also

### Content recognition and interaction in images

Enabling Live Text interactions with images

Add a Live Text interface that enables users to perform actions with text and QR codes that appear in images.

class ImageAnalyzer

An object that finds items in images that people can interact with, such as subjects, text, and QR codes.

class ImageAnalysisInteraction

An interface that enables people to interact with recognized text, barcodes, and other objects in an image.

protocol ImageAnalysisInteractionDelegate

A delegate that handles image-analysis and user-interaction callbacks for an interaction object.

class ImageAnalysisOverlayView

A view that enables people to interact with recognized text, barcodes, and other objects in an image.

protocol ImageAnalysisOverlayViewDelegate

A delegate that handles image-analysis and user-interaction callbacks for an overlay view.

