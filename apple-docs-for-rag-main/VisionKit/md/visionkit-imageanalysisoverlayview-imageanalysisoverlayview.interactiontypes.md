

- VisionKit
- ImageAnalysisOverlayView
-  ImageAnalysisOverlayView.InteractionTypes 

Structure

# ImageAnalysisOverlayView.InteractionTypes

The types of interactions that people can perform with an image.

macOS 13.0+

``` source
struct InteractionTypes
```

## Topics

### Specifying types of interactions

static let automatic: ImageAnalysisOverlayView.InteractionTypes

An option that enables interaction with any type of text, symbols, or subjects that the framework recognizes.

static let textSelection: ImageAnalysisOverlayView.InteractionTypes

An option that enables text selection, copying, and translating.

static let dataDetectors: ImageAnalysisOverlayView.InteractionTypes

An option that enables interaction with text of certain formats, such as URLs, email addresses, and physical addresses.

static let imageSubject: ImageAnalysisOverlayView.InteractionTypes

An option that enables people to click or tap a subject in an image to separate it from the background.

static let visualLookUp: ImageAnalysisOverlayView.InteractionTypes

An option that presents a button for more information on any subjects the framework recognizes in the image.

static let automaticTextOnly: ImageAnalysisOverlayView.InteractionTypes

An option that enables all interaction types except image subjects and Visual Look Up.

### Creating an interaction

init(rawValue: UInt)

Creates an instance from a raw type.

var rawValue: UInt

The corresponding value of the raw type.

### Managing sets

Set properties and methods

The properties and methods that conform to the option set protocol.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Configuring overlay views

var delegate: (any ImageAnalysisOverlayViewDelegate)?

An object that handles image analysis interface callbacks.

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

var preferredInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that people can perform with the image in this overlay view.

var trackingImageView: NSImageView?

The image view that contains the image.

var activeInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that a person actively performs.

