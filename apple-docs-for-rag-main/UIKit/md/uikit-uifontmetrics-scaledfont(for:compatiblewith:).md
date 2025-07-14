

- UIKit
- UIFontMetrics
-  scaledFont(for:compatibleWith:) 

Instance Method

# scaledFont(for:compatibleWith:)

Returns a version of the specified font that adopts the current font metrics and supports the specified traits.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
func scaledFont(
    for font: UIFont,
    compatibleWith traitCollection: UITraitCollection?
) -> UIFont
```

## Parameters 

`font`  

The base font to use when applying the style information. Set the size of your font to the standard Dynamic Type size that you use for the corresponding content. Do not specify a font that has already been scaled; doing so results in an exception.

`traitCollection`  

The trait collection to use when determining compatibility. The returned font is appropriate for use in an interface that adopts the specified traits.

## Return Value

A version of the specified font with the appropriate style information applied to it, and scaled to the current Dynamic Type setting.

## See Also

### Creating Scaled Fonts

Scaling Fonts Automatically

Scale text in your interface automatically using Dynamic Type.

func scaledFont(for: UIFont) -> UIFont

Returns a version of the specified font that adopts the current font metrics.

func scaledFont(for: UIFont, maximumPointSize: CGFloat) -> UIFont

Returns a version of the specified font that adopts the current font metrics and is constrained to the specified maximum size.

func scaledFont(for: UIFont, maximumPointSize: CGFloat, compatibleWith: UITraitCollection?) -> UIFont

Returns a version of the specified font that adopts the current font metrics and is constrained to the specified traits and size.

