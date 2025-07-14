

- VisionKit
- ImageAnalysisInteraction
-  selectedText 

Instance Property

# selectedText

The current selected text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var selectedText: String { get }
```

## See Also

### Accessing text information

var text: String

The text contents of the current image analysis.

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

