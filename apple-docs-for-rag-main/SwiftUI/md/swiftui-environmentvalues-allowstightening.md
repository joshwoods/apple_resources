

- SwiftUI
- EnvironmentValues
-  allowsTightening 

Instance Property

# allowsTightening

A Boolean value that indicates whether inter-character spacing should tighten to fit the text into the available space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var allowsTightening: Bool { get set }
```

## Discussion

The default value is `false`.

## See Also

### Managing text layout

func truncationMode(Text.TruncationMode) -> some View

Sets the truncation mode for lines of text that are too long to fit in the available space.

var truncationMode: Text.TruncationMode

A value that indicates how the layout truncates the last line of text to fit into the available space.

func allowsTightening(Bool) -> some View

Sets whether text in this view can compress the space between characters when necessary to fit text in a line.

func minimumScaleFactor(CGFloat) -> some View

Sets the minimum amount that text in this view scales down to fit in the available space.

var minimumScaleFactor: CGFloat

The minimum permissible proportion to shrink the font size to fit the text into the available space.

func baselineOffset(CGFloat) -> some View

Sets the vertical offset for the text relative to its baseline in this view.

func kerning(CGFloat) -> some View

Sets the spacing, or kerning, between characters for the text in this view.

func tracking(CGFloat) -> some View

Sets the tracking for the text in this view.

func flipsForRightToLeftLayoutDirection(Bool) -> some View

Sets whether this view mirrors its contents horizontally when the layout direction is right-to-left.

enum TextAlignment

An alignment position for text along the horizontal axis.

