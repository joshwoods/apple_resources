

- VisionKit
- ImageAnalysisInteraction
- ImageAnalysisInteraction.InteractionTypes
-  imageSubject 

Type Property

# imageSubject

An option that enables people to use a long-press gesture on a subject in an image to separate it from the background.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
static let imageSubject: ImageAnalysisInteraction.InteractionTypes
```

## Discussion

For more information about image subjects, see ImageAnalysisInteraction.Subject.

## See Also

### Specifying types of interactions

static let automatic: ImageAnalysisInteraction.InteractionTypes

An option that enables interaction with any type of text, symbols, or subjects that the framework recognizes.

static let textSelection: ImageAnalysisInteraction.InteractionTypes

An option that enables text selection, copying, and translating.

static let dataDetectors: ImageAnalysisInteraction.InteractionTypes

An option that enables interaction with text of certain formats, such as URLs, email addresses, and physical addresses.

static let visualLookUp: ImageAnalysisInteraction.InteractionTypes

An option that presents a button for more information on any subjects the framework recognizes in the image.

static let automaticTextOnly: ImageAnalysisInteraction.InteractionTypes

An option that enables all interaction types except image subjects and Visual Look Up.

