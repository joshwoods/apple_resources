

- SwiftUI
- Color
-  mix(with:by:in:) 

Instance Method

# mix(with:by:in:)

Returns a version of self mixed with `rhs` by the amount specified by `fraction`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func mix(
    with rhs: Color,
    by fraction: Double,
    in colorSpace: Gradient.ColorSpace = .perceptual
) -> Color
```

## Parameters 

`rhs`  

The color to mix `self` with.

`fraction`  

The amount of blending, `0.5` means `self` is mixed in equal parts with `rhs`.

`colorSpace`  

The color space used to mix the colors.

## Return Value

A new `Color` based on `self` and `rhs`.

