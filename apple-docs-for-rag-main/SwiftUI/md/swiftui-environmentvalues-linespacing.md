

- SwiftUI
- EnvironmentValues
-  lineSpacing 

Instance Property

# lineSpacing

The distance in points between the bottom of one line fragment and the top of the next.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var lineSpacing: CGFloat { get set }
```

## Discussion

This value is always nonnegative.

## See Also

### Formatting multiline text

func lineSpacing(CGFloat) -> some View

Sets the amount of space between lines of text in this view.

func multilineTextAlignment(TextAlignment) -> some View

Sets the alignment of a text view that contains multiple lines of text.

var multilineTextAlignment: TextAlignment

An environment value that indicates how a text view aligns its lines when the content wraps or contains newlines.

