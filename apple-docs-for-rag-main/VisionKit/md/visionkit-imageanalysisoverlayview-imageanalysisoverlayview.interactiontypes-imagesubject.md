

- VisionKit
- ImageAnalysisOverlayView
- ImageAnalysisOverlayView.InteractionTypes
-  imageSubject 

Type Property

# imageSubject

An option that enables people to click or tap a subject in an image to separate it from the background.

macOS 13.0+

``` source
static let imageSubject: ImageAnalysisOverlayView.InteractionTypes
```

## Discussion

For more information about image subjects, see ImageAnalysisOverlayView.Subject.

## See Also

### Specifying types of interactions

static let automatic: ImageAnalysisOverlayView.InteractionTypes

An option that enables interaction with any type of text, symbols, or subjects that the framework recognizes.

static let textSelection: ImageAnalysisOverlayView.InteractionTypes

An option that enables text selection, copying, and translating.

static let dataDetectors: ImageAnalysisOverlayView.InteractionTypes

An option that enables interaction with text of certain formats, such as URLs, email addresses, and physical addresses.

static let visualLookUp: ImageAnalysisOverlayView.InteractionTypes

An option that presents a button for more information on any subjects the framework recognizes in the image.

static let automaticTextOnly: ImageAnalysisOverlayView.InteractionTypes

An option that enables all interaction types except image subjects and Visual Look Up.

