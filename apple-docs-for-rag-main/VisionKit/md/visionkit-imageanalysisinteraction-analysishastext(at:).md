

- VisionKit
- ImageAnalysisInteraction
-  analysisHasText(at:) 

Instance Method

# analysisHasText(at:)

Returns a Boolean value that indicates whether the analysis finds text at the specified point.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final func analysisHasText(at point: CGPoint) -> Bool
```

## Parameters 

`point`  

A point in the image, in view coordinates.

## Return Value

`true` if text exists at `point`; otherwise, `false`.

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

var hasActiveTextSelection: Bool

A Boolean value that indicates whether a person or the app has text selected within the image.

func hasDataDetector(at: CGPoint) -> Bool

Returns a Boolean value that indicates whether the analysis detects data at the specified point.

