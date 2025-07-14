

- VisionKit
- ImageAnalysisInteraction
-  ImageAnalysisInteraction.InteractionTypes 

Structure

# ImageAnalysisInteraction.InteractionTypes

The types of interactions that people can perform with an image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
struct InteractionTypes
```

## Topics

### Specifying types of interactions

static let automatic: ImageAnalysisInteraction.InteractionTypes

An option that enables interaction with any type of text, symbols, or subjects that the framework recognizes.

static let textSelection: ImageAnalysisInteraction.InteractionTypes

An option that enables text selection, copying, and translating.

static let dataDetectors: ImageAnalysisInteraction.InteractionTypes

An option that enables interaction with text of certain formats, such as URLs, email addresses, and physical addresses.

static let imageSubject: ImageAnalysisInteraction.InteractionTypes

An option that enables people to use a long-press gesture on a subject in an image to separate it from the background.

static let visualLookUp: ImageAnalysisInteraction.InteractionTypes

An option that presents a button for more information on any subjects the framework recognizes in the image.

static let automaticTextOnly: ImageAnalysisInteraction.InteractionTypes

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

### Configuring an image interaction

var delegate: (any ImageAnalysisInteractionDelegate)?

The delegate that handles the interaction callbacks.

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

var view: UIView?

The view that uses this interaction.

var preferredInteractionTypes: ImageAnalysisInteraction.InteractionTypes

The types of interactions that people can perform with the image.

var activeInteractionTypes: ImageAnalysisInteraction.InteractionTypes

The types of interactions that a person actively performs.

