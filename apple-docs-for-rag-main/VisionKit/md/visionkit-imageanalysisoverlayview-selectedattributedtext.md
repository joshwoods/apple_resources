

- VisionKit
- ImageAnalysisOverlayView
-  selectedAttributedText 

Instance Property

# selectedAttributedText

The current selected attributed text.

macOS 14.0+

``` source
@MainActor
final var selectedAttributedText: AttributedString { get }
```

## See Also

### Accessing text information

var text: String

The text contents of the current image analysis.

var selectedText: String

The current selected text.

var hasActiveTextSelection: Bool

A Boolean value that indicates whether a person or the app has text selected within the image.

func analysisHasText(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether the analysis finds text at the specified point.

func hasText(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether active text exists at the specified point.

func hasDataDetector(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether the analysis detects data at the specified point.

