

- AppKit
- NSFontManager
-  convert(\_:) 

Instance Method

# convert(\_:)

Converts the given font according to the object that initiated a font change, typically the Font panel or Font menu.

macOS

``` source
func convert(_ fontObj: NSFont) -> NSFont
```

## Parameters 

`fontObj`  

The font to convert.

## Return Value

The converted font, or `aFont` itself if the conversion isn’t possible.

## Discussion

This method is invoked in response to an action message such as addFontTrait(_:) or modifyFontViaPanel(_:). These initiating methods cause the font manager to query the sender for the action to take and the traits to change. See Converting Fonts Manually for more information.

## See Also

### Related Documentation

func convert(NSFont, toFamily: String) -> NSFont

Returns a font whose traits are as similar as possible to those of the given font except for the font family, which is changed to the given family.

func convert(NSFont, toSize: CGFloat) -> NSFont

Returns a font object whose traits are the same as those of the given font, except for the size, which is changed to the given size.

func convert(NSFont, toHaveTrait: NSFontTraitMask) -> NSFont

Returns a new version of the font object containing a single additional trait.

func convert(NSFont, toNotHaveTrait: NSFontTraitMask) -> NSFont

Returns a new version of a font object without the specified traits.

func convertWeight(Bool, of: NSFont) -> NSFont

Returns a font object whose weight is greater or lesser than that of the given font.

func convert(NSFont, toFace: String) -> NSFont?

Returns a font whose traits are as similar as possible to those of the given font except for the typeface, which is changed to the given typeface.

