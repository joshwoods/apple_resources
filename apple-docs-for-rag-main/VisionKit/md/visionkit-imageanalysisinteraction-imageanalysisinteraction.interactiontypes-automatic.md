

- VisionKit
- ImageAnalysisInteraction
- ImageAnalysisInteraction.InteractionTypes
-  automatic 

Type Property

# automatic

An option that enables interaction with any type of text, symbols, or subjects that the framework recognizes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
static let automatic: ImageAnalysisInteraction.InteractionTypes
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

People can select text to perform actions, and after tapping the Live Text button, they can interact with data detectors. If the allowLongPressForDataDetectorsInTextMode property is `true`, a person can touch and hold text to activate data detectors without tapping the Live Text button.

## See Also

### Specifying types of interactions

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

