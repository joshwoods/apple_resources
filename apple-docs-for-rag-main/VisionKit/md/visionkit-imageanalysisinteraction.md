

- VisionKit
-  ImageAnalysisInteraction 

Class

# ImageAnalysisInteraction

An interface that enables people to interact with recognized text, barcodes, and other objects in an image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor @objc
final class ImageAnalysisInteraction
```

## Mentioned in 

Enabling Live Text interactions with images

## Overview

This class enables people to interact with specific content types (ImageAnalysisInteraction.InteractionTypes) that the framework identifies in an image. For example:

- The Live Text interface enables them to select any text present in the image (textSelection), or invoke a URL (dataDetectors). The text selection UI offers framework-standard buttons for copying selected text, or looking it up on the web for more information.

- The *subject lift* feature identifies a wide variety of objects, or *subjects*, in images with the imageSubject interaction type, and provides your app with an image of the objects with the background removed. The visualLookUp type supplements this feature by adding a button in the bottom corner of the view that people can click or tap for more information about the recognized subjects.

## Configure the interface and begin interaction

This class conforms to the UIInteraction protocol. To connect the interface with an image that your app displays, call addInteraction(_:) on your app’s image view and pass in a new instance of this class.

Choose the items that the framework recognizes in an image by configuring the preferredInteractionTypes property. To recognize all types of content, specify the automatic option, or choose a combination of types by assigning an array:

```
interaction.preferredInteractionTypes = [.textSelection, .imageSubject]
```

To begin interaction, call one of the ImageAnalyzer class’s `analyze` methods, such as analyze(_:configuration:) and set the result onto this class’s analysis property.

You can take more control over the interaction or provide details about your app’s image view by implementing a delegate (ImageAnalysisInteractionDelegate) and assigning it to the delegate property. If your image view isn’t an instance of UIImageView, your app needs to define the interactive area within the image by implementing the contentsRect(for:) method.

## Topics

### Creating an image interaction

init()

Creates an interaction for Live Text actions with items in an image.

convenience init(any ImageAnalysisInteractionDelegate)

Creates an interaction for Live Text actions with the specified delegate.

### Configuring an image interaction

var delegate: (any ImageAnalysisInteractionDelegate)?

The delegate that handles the interaction callbacks.

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

var view: UIView?

The view that uses this interaction.

var preferredInteractionTypes: ImageAnalysisInteraction.InteractionTypes

The types of interactions that people can perform with the image.

struct InteractionTypes

The types of interactions that people can perform with an image.

var activeInteractionTypes: ImageAnalysisInteraction.InteractionTypes

The types of interactions that a person actively performs.

### Responding to view events

func willMove(to: UIView?)

Performs an action before the view adds or removes the interaction from its interaction array.

func didMove(to: UIView?)

Performs an action after the view adds or removes the interaction from its interaction array.

### Accessing text information

var text: String

The text contents of the current image analysis.

var selectedText: String

The current selected text.

var selectedAttributedText: AttributedString

The current selected attributed text.

func hasText(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether active text exists at the specified point.

var hasActiveTextSelection: Bool

A Boolean value that indicates whether a person or the app has text selected within the image.

func analysisHasText(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether the analysis finds text at the specified point.

func hasDataDetector(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether the analysis detects data at the specified point.

### Managing text selection

var selectedRanges: [Range&lt;String.Index>]

Sets selected text ranges.

func resetTextSelection()

Removes a person’s text selection from the interface.

### Accessing image subjects

var subjects: Set&lt;ImageAnalysisInteraction.Subject>

The set of all subjects the framework identifies in an image.

struct Subject

An area of interest in an image that the framework identifies as a primary focal point.

func image(for: Set&lt;ImageAnalysisInteraction.Subject>) async throws -> UIImage

Provides an image asynchronously that contains the given subjects with the background removed.

func subject(at: CGPoint) async -> ImageAnalysisInteraction.Subject?

Returns the subject at the given point within the interaction’s image, if one exists.

### Managing image subjects

var highlightedSubjects: Set&lt;ImageAnalysisInteraction.Subject>

All highlighted subjects in the interaction image.

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

A Boolean value that indicates whether the interaction highlights actionable text or data the analyzer detects in text.

### Customizing the interface

var allowLongPressForDataDetectorsInTextMode: Bool

A Boolean value that indicates whether people can press and hold text to activate data detectors.

func setSupplementaryInterfaceHidden(Bool, animated: Bool)

Hides or shows supplementary interface objects, such as the Live Action button and Quick Actions, depending on the item type.

var supplementaryInterfaceContentInsets: UIEdgeInsets

The distances the edges of content are inset from the supplementary interface.

var supplementaryInterfaceFont: UIFont?

The font to use for the supplementary interface.

### Managing custom image views

var contentsRect: CGRect

A rectangle, in unit coordinate space, that describes the content area of the interaction.

func setContentsRectNeedsUpdate()

Informs the view that contains the image when the layout changes and the view needs to reload its content.

### Errors

enum SubjectUnavailable

Error conditions that can occur during subject analysis.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIInteraction

## See Also

### Content recognition and interaction in images

Enabling Live Text interactions with images

Add a Live Text interface that enables users to perform actions with text and QR codes that appear in images.

class ImageAnalyzer

An object that finds items in images that people can interact with, such as subjects, text, and QR codes.

class ImageAnalysis

An object that represents the results of analyzing an image, and provides the input for the Live Text interface object.

protocol ImageAnalysisInteractionDelegate

A delegate that handles image-analysis and user-interaction callbacks for an interaction object.

class ImageAnalysisOverlayView

A view that enables people to interact with recognized text, barcodes, and other objects in an image.

protocol ImageAnalysisOverlayViewDelegate

A delegate that handles image-analysis and user-interaction callbacks for an overlay view.

