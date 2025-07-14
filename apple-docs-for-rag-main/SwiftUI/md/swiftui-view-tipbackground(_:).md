

- SwiftUI
- View
-  tipBackground(\_:) 

Instance Method

# tipBackground(\_:)

Sets the tip’s view background to a style. Currently this only applies to inline tips, not popover tips.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
func tipBackground(_ style: some ShapeStyle) -> some View
```

## Parameters 

`style`  

An instance of a type that conforms to `ShapeStyle` that SwiftUI draws behind the modified view.

## Return Value

A view with the specified style drawn behind it.

## See Also

### Providing tips

func popoverTip((any Tip)?, arrowEdge: Edge?, action: (Tips.Action) -> Void) -> some View

Presents a popover tip on the modified view.

func tipCornerRadius(CGFloat, antialiased: Bool) -> some View

Sets the corner radius for an inline tip view.

func tipImageSize(CGSize) -> some View

Sets the size for a tip’s image.

func tipViewStyle(some TipViewStyle) -> some View

Sets the given style for TipView within the view hierarchy.

func tipImageStyle&lt;S>(S) -> some View

Sets the style for a tip’s image.

func tipImageStyle&lt;S1, S2>(S1, S2) -> some View

Sets the style for a tip’s image.

func tipImageStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the style for a tip’s image.

