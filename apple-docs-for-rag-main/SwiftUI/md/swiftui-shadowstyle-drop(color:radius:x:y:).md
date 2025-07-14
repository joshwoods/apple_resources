

- SwiftUI
- ShadowStyle
-  drop(color:radius:x:y:) 

Type Method

# drop(color:radius:x:y:)

Creates a custom drop shadow style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func drop(
    color: Color = .init(.sRGBLinear, white: 0, opacity: 0.33),
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

Drop shadows draw behind the source content by blurring, tinting and offsetting its per-pixel alpha values.

## See Also

### Getting shadow styles

static func inner(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> ShadowStyle

Creates a custom inner shadow style.

