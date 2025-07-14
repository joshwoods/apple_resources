

- AppKit
- NSFontManager
-  convert(\_:toSize:) 

Instance Method

# convert(\_:toSize:)

Returns a font object whose traits are the same as those of the given font, except for the size, which is changed to the given size.

macOS

``` source
func convert(
    _ fontObj: NSFont,
    toSize size: CGFloat
) -> NSFont
```

## Parameters 

`fontObj`  

The font whose traits are matched.

`size`  

The new font size.

## Return Value

A font with matching traits except in the new size, or `aFont` if it can’t be converted.

## See Also

### Related Documentation

func convert(NSFont) -> NSFont

Converts the given font according to the object that initiated a font change, typically the Font panel or Font menu.

### Converting Fonts Manually

func convert(NSFont, toFace: String) -> NSFont?

Returns a font whose traits are as similar as possible to those of the given font except for the typeface, which is changed to the given typeface.

func convert(NSFont, toFamily: String) -> NSFont

Returns a font whose traits are as similar as possible to those of the given font except for the font family, which is changed to the given family.

func convert(NSFont, toHaveTrait: NSFontTraitMask) -> NSFont

Returns a new version of the font object containing a single additional trait.

func convert(NSFont, toNotHaveTrait: NSFontTraitMask) -> NSFont

Returns a new version of a font object without the specified traits.

func convertWeight(Bool, of: NSFont) -> NSFont

Returns a font object whose weight is greater or lesser than that of the given font.

var currentFontAction: NSFontAction

The current font conversion action.

func convertFontTraits(NSFontTraitMask) -> NSFontTraitMask

Converts font traits to a new traits mask value.

