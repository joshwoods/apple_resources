

- AppKit
- NSFontManager
-  convert(\_:toFace:) 

Instance Method

# convert(\_:toFace:)

Returns a font whose traits are as similar as possible to those of the given font except for the typeface, which is changed to the given typeface.

macOS

``` source
func convert(
    _ fontObj: NSFont,
    toFace typeface: String
) -> NSFont?
```

## Parameters 

`fontObj`  

The font whose traits are matched.

`typeface`  

The new typeface; a fully specified family-face name, such as Helvetica-BoldOblique or Times-Roman.

## Return Value

A font with matching traits and the given typeface, or `aFont` if it can’t be converted.

## Discussion

This method attempts to match the weight and posture of `aFont` as closely as possible. Italic is mapped to Oblique, for example. Weights are mapped based on an approximate numeric scale of 0 to 15.

## See Also

### Related Documentation

func convert(NSFont) -> NSFont

Converts the given font according to the object that initiated a font change, typically the Font panel or Font menu.

### Converting Fonts Manually

func convert(NSFont, toFamily: String) -> NSFont

Returns a font whose traits are as similar as possible to those of the given font except for the font family, which is changed to the given family.

func convert(NSFont, toHaveTrait: NSFontTraitMask) -> NSFont

Returns a new version of the font object containing a single additional trait.

func convert(NSFont, toNotHaveTrait: NSFontTraitMask) -> NSFont

Returns a new version of a font object without the specified traits.

func convert(NSFont, toSize: CGFloat) -> NSFont

Returns a font object whose traits are the same as those of the given font, except for the size, which is changed to the given size.

func convertWeight(Bool, of: NSFont) -> NSFont

Returns a font object whose weight is greater or lesser than that of the given font.

var currentFontAction: NSFontAction

The current font conversion action.

func convertFontTraits(NSFontTraitMask) -> NSFontTraitMask

Converts font traits to a new traits mask value.

