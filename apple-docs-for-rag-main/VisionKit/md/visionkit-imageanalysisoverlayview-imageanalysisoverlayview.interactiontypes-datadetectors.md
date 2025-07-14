

- VisionKit
- ImageAnalysisOverlayView
- ImageAnalysisOverlayView.InteractionTypes
-  dataDetectors 

Type Property

# dataDetectors

An option that enables interaction with text of certain formats, such as URLs, email addresses, and physical addresses.

macOS 13.0+

``` source
static let dataDetectors: ImageAnalysisOverlayView.InteractionTypes
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

People interact with *data detectors*, or UI that highlights each instance of the recognized formats in text that’s on an image. The data detectors appear without a Live Text button, because people can’t interact with other text with this option.

## See Also

### Specifying types of interactions

static let automatic: ImageAnalysisOverlayView.InteractionTypes

An option that enables interaction with any type of text, symbols, or subjects that the framework recognizes.

static let textSelection: ImageAnalysisOverlayView.InteractionTypes

An option that enables text selection, copying, and translating.

static let imageSubject: ImageAnalysisOverlayView.InteractionTypes

An option that enables people to click or tap a subject in an image to separate it from the background.

static let visualLookUp: ImageAnalysisOverlayView.InteractionTypes

An option that presents a button for more information on any subjects the framework recognizes in the image.

static let automaticTextOnly: ImageAnalysisOverlayView.InteractionTypes

An option that enables all interaction types except image subjects and Visual Look Up.

