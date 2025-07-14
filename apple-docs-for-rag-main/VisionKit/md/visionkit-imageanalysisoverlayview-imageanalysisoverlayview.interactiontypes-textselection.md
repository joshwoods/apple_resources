

- VisionKit
- ImageAnalysisOverlayView
- ImageAnalysisOverlayView.InteractionTypes
-  textSelection 

Type Property

# textSelection

An option that enables text selection, copying, and translating.

macOS 13.0+

``` source
static let textSelection: ImageAnalysisOverlayView.InteractionTypes
```

## See Also

### Specifying types of interactions

static let automatic: ImageAnalysisOverlayView.InteractionTypes

An option that enables interaction with any type of text, symbols, or subjects that the framework recognizes.

static let dataDetectors: ImageAnalysisOverlayView.InteractionTypes

An option that enables interaction with text of certain formats, such as URLs, email addresses, and physical addresses.

static let imageSubject: ImageAnalysisOverlayView.InteractionTypes

An option that enables people to click or tap a subject in an image to separate it from the background.

static let visualLookUp: ImageAnalysisOverlayView.InteractionTypes

An option that presents a button for more information on any subjects the framework recognizes in the image.

static let automaticTextOnly: ImageAnalysisOverlayView.InteractionTypes

An option that enables all interaction types except image subjects and Visual Look Up.

