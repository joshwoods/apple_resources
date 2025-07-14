

- VisionKit
- ImageAnalysisInteraction
-  hasActiveTextSelection 

Instance Property

# hasActiveTextSelection

A Boolean value that indicates whether a person or the app has text selected within the image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var hasActiveTextSelection: Bool { get }
```

## Discussion

If textSelection is an active interaction type, a person can select text using a standard input method and the app can select text through the selectedRanges property. If neither a person nor the app select any text, then this property returns `false`.

## See Also

### Accessing text information

var text: String

The text contents of the current image analysis.

var selectedText: String

The current selected text.

var selectedAttributedText: AttributedString

The current selected attributed text.

func hasText(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether active text exists at the specified point.

func analysisHasText(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether the analysis finds text at the specified point.

func hasDataDetector(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether the analysis detects data at the specified point.

