

- AppKit
- NSFontManager
-  convertFontTraits(\_:) 

Instance Method

# convertFontTraits(\_:)

Converts font traits to a new traits mask value.

macOS 10.5+

``` source
func convertFontTraits(_ traits: NSFontTraitMask) -> NSFontTraitMask
```

## Parameters 

`traits`  

The current font traits.

## Return Value

The new traits mask value to be used by convert(_:).

## Discussion

This method is intended to be invoked to query the font traits while the action message (usually changeFont:) is being invoked when the current font action is either NSFontAction.addTraitFontAction or NSFontAction.removeTraitFontAction.

## See Also

### Converting Fonts Manually

func convert(NSFont, toFace: String) -> NSFont?

Returns a font whose traits are as similar as possible to those of the given font except for the typeface, which is changed to the given typeface.

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

