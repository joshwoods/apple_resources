

- SwiftUI
- View
-  tipImageStyle(\_:) 

Instance Method

# tipImageStyle(\_:)

Sets the style for a tip’s image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor @preconcurrency
func tipImageStyle(_ style: S) -> some View where S : ShapeStyle
```

## See Also

### Providing tips

func popoverTip((any Tip)?, arrowEdge: Edge?, action: (Tips.Action) -> Void) -> some View

Presents a popover tip on the modified view.

func tipBackground(some ShapeStyle) -> some View

Sets the tip’s view background to a style. Currently this only applies to inline tips, not popover tips.

func tipCornerRadius(CGFloat, antialiased: Bool) -> some View

Sets the corner radius for an inline tip view.

func tipImageSize(CGSize) -> some View

Sets the size for a tip’s image.

func tipViewStyle(some TipViewStyle) -> some View

Sets the given style for TipView within the view hierarchy.

func tipImageStyle&lt;S1, S2>(S1, S2) -> some View

Sets the style for a tip’s image.

func tipImageStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the style for a tip’s image.

