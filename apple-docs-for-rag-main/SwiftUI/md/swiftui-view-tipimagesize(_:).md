

- SwiftUI
- View
-  tipImageSize(\_:) 

Instance Method

# tipImageSize(\_:)

Sets the size for a tip’s image.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
func tipImageSize(_ size: CGSize) -> some View
```

## See Also

### Providing tips

func popoverTip((any Tip)?, arrowEdge: Edge?, action: (Tips.Action) -> Void) -> some View

Presents a popover tip on the modified view.

func tipBackground(some ShapeStyle) -> some View

Sets the tip’s view background to a style. Currently this only applies to inline tips, not popover tips.

func tipCornerRadius(CGFloat, antialiased: Bool) -> some View

Sets the corner radius for an inline tip view.

func tipViewStyle(some TipViewStyle) -> some View

Sets the given style for TipView within the view hierarchy.

func tipImageStyle&lt;S>(S) -> some View

Sets the style for a tip’s image.

func tipImageStyle&lt;S1, S2>(S1, S2) -> some View

Sets the style for a tip’s image.

func tipImageStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the style for a tip’s image.

