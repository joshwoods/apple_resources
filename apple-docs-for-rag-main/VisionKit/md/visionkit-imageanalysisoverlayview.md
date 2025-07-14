

- VisionKit
-  ImageAnalysisOverlayView 

Class

# ImageAnalysisOverlayView

A view that enables people to interact with recognized text, barcodes, and other objects in an image.

macOS 13.0+

``` source
@MainActor @objc
final class ImageAnalysisOverlayView
```

## Mentioned in 

Enabling Live Text interactions with images

## Overview

This class enables people to interact with specific content types (ImageAnalysisOverlayView.InteractionTypes) that the framework identifies in an image. For example:

- The Live Text interface enables them to select any text present in the image (textSelection), or invoke a URL (dataDetectors). The text selection UI offers framework-standard buttons for copying selected text, or looking it up on the web for more information.

- The *subject lift* feature identifies a wide variety of objects, or *subjects*, in images with the imageSubject interaction type, and provides your app with an image of the objects with the background removed. The visualLookUp type supplements this feature by adding a button in the bottom corner of the view that people can click or tap for more information about the recognized subjects.

## Configure the interface and begin interaction

To connect the interface with an image that your app displays, add a new instance of this class as a subview to your app’s image view.

Choose the items that the framework recognizes in an image by configuring the preferredInteractionTypes property. To recognize all types of content, specify the automatic option, or choose a combination of types by assigning an array:

```
overlayView.preferredInteractionTypes = [.textSelection, .imageSubject]
```

To begin interaction, call one of the ImageAnalyzer class’s `analyze` methods, such as analyze(_:configuration:) and set the result onto this class’s analysis property.

You can take more control over the interaction or provide details about your app’s image view by implementing a delegate (ImageAnalysisInteractionDelegate) and assigning it to the delegate property. Your app needs to define the interactive area within the image either by setting the trackingImageView property, or by implementing the delegate’s contentsRect(for:) method.

## Topics

### Creating overlay views

convenience init(any ImageAnalysisOverlayViewDelegate)

Creates an overlay view with the specified delegate object.

init(frame: NSRect)

Creates an overlay view with the specified frame rectangle.

init?(coder: NSCoder)

Creates an overlay view from data in a coder object.

### Configuring overlay views

var delegate: (any ImageAnalysisOverlayViewDelegate)?

An object that handles image analysis interface callbacks.

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

var preferredInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that people can perform with the image in this overlay view.

struct InteractionTypes

The types of interactions that people can perform with an image.

var trackingImageView: NSImageView?

The image view that contains the image.

var activeInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that a person actively performs.

### Responding to view events

func viewDidMoveToSuperview()

Notifies your app when the view initially appears.

### Accessing text information

var text: String

The text contents of the current image analysis.

var selectedText: String

The current selected text.

var selectedAttributedText: AttributedString

The current selected attributed text.

var hasActiveTextSelection: Bool

A Boolean value that indicates whether a person or the app has text selected within the image.

func analysisHasText(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether the analysis finds text at the specified point.

func hasText(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether active text exists at the specified point.

func hasDataDetector(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether the analysis detects data at the specified point.

### Managing text selection

var selectedRanges: [Range&lt;String.Index>]

The current selected ranges.

func resetSelection()

Removes a person’s text selection from the interface.

### Accessing image subjects

var subjects: Set&lt;ImageAnalysisOverlayView.Subject>

The set of all subjects the framework identifies in an image.

struct Subject

An area of interest in an image that the framework identifies as a primary focal point.

func image(for: Set&lt;ImageAnalysisOverlayView.Subject>) async throws -> NSImage

Provides an image asynchronously that contains the given subjects with the background removed.

func subject(at: CGPoint) async -> ImageAnalysisOverlayView.Subject?

Returns the subject at the given point within the overlay view’s image, if one exists.

### Managing image subjects

func beginSubjectAnalysisIfNecessary()

Begins subject analysis on the overlay view’s image.

var highlightedSubjects: Set&lt;ImageAnalysisOverlayView.Subject>

All highlighted subjects in the overlay view’s image.

### Querying the interface state

var liveTextButtonVisible: Bool

A Boolean value that indicates whether the Live Text button appears.

var isSupplementaryInterfaceHidden: Bool

A Boolean value that indicates whether the view hides supplementary interface objects.

func hasInteractiveItem(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether active text, data detectors, or supplementary interface objects exist at the specified point.

func hasSupplementaryInterface(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether supplementary interface objects exist at the specified point.

var selectableItemsHighlighted: Bool

A Boolean value that indicates whether the overlay view highlights actionable text or data that the analyzer detects in text.

### Customizing the interface

func setSupplementaryInterfaceHidden(Bool, animated: Bool)

Hides or shows supplementary interface objects, such as the Live Text button and the interface for Quick Actions, depending on the item type.

var supplementaryInterfaceContentInsets: NSEdgeInsets

The distances the edges of content are inset from the supplementary interface.

var supplementaryInterfaceFont: NSFont?

The font to use for the supplementary interface.

struct MenuTag

Tags that enable your app to manage image-analysis context menu items.

### Managing custom image views

var contentsRect: CGRect

Returns the rectangle, in unit coordinates, that contains the image within the superview.

func setContentsRectNeedsUpdate()

Informs the view that contains the image when the layout changes and the view needs to reload its content.

### Errors

enum SubjectUnavailable

Error conditions that can occur during subject analysis.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification

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

protocol ImageAnalysisOverlayViewDelegate

A delegate that handles image-analysis and user-interaction callbacks for an overlay view.

