

- UIKit
- UIFontMetrics
-  scaledFont(for:maximumPointSize:compatibleWith:) 

Instance Method

# scaledFont(for:maximumPointSize:compatibleWith:)

Returns a version of the specified font that adopts the current font metrics and is constrained to the specified traits and size.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
func scaledFont(
    for font: UIFont,
    maximumPointSize: CGFloat,
    compatibleWith traitCollection: UITraitCollection?
) -> UIFont
```

## Parameters 

`font`  

The base font to use when applying the style information. Set the size of your font to the standard Dynamic Type size that you use for the corresponding content. Do not specify a font that has already been scaled; doing so results in an exception.

`maximumPointSize`  

The maximum point size allowed for the font. Use this value to constrain the font to the specified size when your interface cannot accommodate text that is any larger.

`traitCollection`  

The trait collection to use when determining compatibility. The returned font is appropriate for use in an interface that adopts the specified traits.

## Return Value

A version of the specified font with the appropriate style information applied to it, and scaled appropriately for the specified settings.

## See Also

### Creating Scaled Fonts

Scaling Fonts Automatically

Scale text in your interface automatically using Dynamic Type.

func scaledFont(for: UIFont) -> UIFont

Returns a version of the specified font that adopts the current font metrics.

func scaledFont(for: UIFont, compatibleWith: UITraitCollection?) -> UIFont

Returns a version of the specified font that adopts the current font metrics and supports the specified traits.

func scaledFont(for: UIFont, maximumPointSize: CGFloat) -> UIFont

Returns a version of the specified font that adopts the current font metrics and is constrained to the specified maximum size.

