

- UIKit
- UIFontDescriptor
- UIFontDescriptor.TraitKey
-  width 

Type Property

# width

The inter-glyph spacing of the font.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
static let width: UIFontDescriptor.TraitKey
```

## Discussion

The value of this key is an NSNumber object. The valid value range is from `-1.0` to `1.0`. The value of `0.0` corresponds to the regular glyph spacing.

## See Also

### Font traits

static let slant: UIFontDescriptor.TraitKey

The relative slant angle of the font.

static let symbolic: UIFontDescriptor.TraitKey

The symbolic font traits.

static let weight: UIFontDescriptor.TraitKey

The numerical value that corresponds to a font face.

