

- SwiftUI
- ShadowStyle
-  inner(color:radius:x:y:) 

Type Method

# inner(color:radius:x:y:)

Creates a custom inner shadow style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func inner(
    color: Color = .init(.sRGBLinear, white: 0, opacity: 0.55),
    radius: CGFloat,
    x: CGFloat = 0,
    y: CGFloat = 0
) -> ShadowStyle
```

## Parameters 

`color`  

The shadow’s color.

`radius`  

The shadow’s size.

`x`  

A horizontal offset you use to position the shadow relative to this view.

`y`  

A vertical offset you use to position the shadow relative to this view.

## Return Value

A new shadow style.

## Discussion

Inner shadows draw on top of the source content by blurring, tinting, inverting and offsetting its per-pixel alpha values.

## See Also

### Getting shadow styles

static func drop(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> ShadowStyle

Creates a custom drop shadow style.

