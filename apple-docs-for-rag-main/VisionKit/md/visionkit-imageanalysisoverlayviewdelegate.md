

- VisionKit
-  ImageAnalysisOverlayViewDelegate 

Protocol

# ImageAnalysisOverlayViewDelegate

A delegate that handles image-analysis and user-interaction callbacks for an overlay view.

macOS 13.0+

``` source
@MainActor
protocol ImageAnalysisOverlayViewDelegate : AnyObject
```

## Mentioned in 

Enabling Live Text interactions with images

## Overview

The delegate of an ImageAnalysisOverlayView object implements this protocol to provide interface details and to customize the response for a person’s interaction.

## Topics

### Providing interface details

func contentView(for: ImageAnalysisOverlayView) -> NSView?

Provides the view that contains the image.

**Required** Default implementation provided.

func contentsRect(for: ImageAnalysisOverlayView) -> CGRect

Returns the rectangle, in unit coordinate space, that contains the image within the view.

**Required** Default implementation provided.

### Starting the interaction

func overlayView(ImageAnalysisOverlayView, shouldBeginAt: CGPoint, forAnalysisType: ImageAnalysisOverlayView.InteractionTypes) -> Bool

Provides a Boolean value that indicates whether the interaction can begin at the given point.

**Required** Default implementation provided.

### Tracking interface changes

func overlayView(ImageAnalysisOverlayView, liveTextButtonDidChangeToVisible: Bool)

Notifies your app when the Live Text button’s visibility changes.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, highlightSelectedItemsDidChange: Bool)

Notifies your app when recognized items in the image appear highlighted as a result of a person clicking or tapping the Live Text button.

**Required** Default implementation provided.

func textSelectionDidChange(ImageAnalysisOverlayView)

Notifies your app when the interaction’s text selection changes.

**Required** Default implementation provided.

### Responding to key and menu events

func overlayView(ImageAnalysisOverlayView, shouldHandleKeyDownEvent: NSEvent) -> Bool

Returns a Boolean value that indicates whether the overlay view consumes the given key-down event.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, shouldShowMenuForEvent: NSEvent, atPoint: CGPoint) -> Bool

Provides a Boolean value that indicates whether the overlay view shows a menu for the given event.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, menu: NSMenu, willHighlight: NSMenuItem?)

Notifies your app that the given menu item is highlighted.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, willOpen: NSMenu)

Notifies your app that a given menu is opening imminently.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, didClose: NSMenu)

Notifies your app that the given menu closed.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, needsUpdate: NSMenu)

Notifies your app that the given menu needs updating.

**Required** Default implementation provided.

func overlayView(ImageAnalysisOverlayView, updatedMenuFor: NSMenu, for: NSEvent, at: CGPoint) -> NSMenu

Notifies your app before the framework presents a context menu.

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

protocol ImageAnalysisInteractionDelegate

A delegate that handles image-analysis and user-interaction callbacks for an interaction object.

class ImageAnalysisOverlayView

A view that enables people to interact with recognized text, barcodes, and other objects in an image.

