

- VisionKit
-  ImageAnalysisInteractionDelegate 

Protocol

# ImageAnalysisInteractionDelegate

A delegate that handles image-analysis and user-interaction callbacks for an interaction object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
protocol ImageAnalysisInteractionDelegate : AnyObject
```

## Mentioned in 

Enabling Live Text interactions with images

## Overview

The delegate of an ImageAnalysisInteraction object implements this protocol to provide interface details and to customize the response for a person’s interaction.

## Topics

### Providing interface details

func contentView(for: ImageAnalysisInteraction) -> UIView?

Provides the view that contains the image.

**Required** Default implementation provided.

func contentsRect(for: ImageAnalysisInteraction) -> CGRect

Returns the rectangle, in unit coordinates, that contains the image within the view.

**Required** Default implementation provided.

func presentingViewController(for: ImageAnalysisInteraction) -> UIViewController?

Provides the view controller that presents the interface objects.

**Required** Default implementation provided.

### Starting the interaction

func interaction(ImageAnalysisInteraction, shouldBeginAt: CGPoint, for: ImageAnalysisInteraction.InteractionTypes) -> Bool

Provides a Boolean value that indicates whether the interaction can begin at the given point.

**Required** Default implementation provided.

### Tracking interface changes

func interaction(ImageAnalysisInteraction, liveTextButtonDidChangeToVisible: Bool)

Notifies your app when the Live Text button’s visibility changes.

**Required** Default implementation provided.

func interaction(ImageAnalysisInteraction, highlightSelectedItemsDidChange: Bool)

Notifies your app when recognized items in the image appear highlighted as a result of a person tapping the Live Text button.

**Required** Default implementation provided.

func textSelectionDidChange(ImageAnalysisInteraction)

Notifies your app when the interaction’s text selection changes.

**Required** Default implementation provided.

## See Also

### Content recognition and interaction in images

Enabling Live Text interactions with images

Add a Live Text interface that enables users to perform actions with text and QR codes that appear in images.

class ImageAnalyzer

An object that finds items in images that people can interact with, such as subjects, text, and QR codes.

class ImageAnalysis

An object that represents the results of analyzing an image, and provides the input for the Live Text interface object.

class ImageAnalysisInteraction

An interface that enables people to interact with recognized text, barcodes, and other objects in an image.

class ImageAnalysisOverlayView

A view that enables people to interact with recognized text, barcodes, and other objects in an image.

protocol ImageAnalysisOverlayViewDelegate

A delegate that handles image-analysis and user-interaction callbacks for an overlay view.

