

- UIKit
- UIFontDescriptor
- UIFontDescriptor.TraitKey
-  slant 

Type Property

# slant

The relative slant angle of the font.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
static let slant: UIFontDescriptor.TraitKey
```

## Discussion

The value of this key is an NSNumber object. The valid value range is from `-1.0` to `1.0`. The value of `0.0` corresponds to `0` degree clockwise rotation from the vertical and `1.0` corresponds to `30` degrees clockwise rotation.

## See Also

### Font traits

static let symbolic: UIFontDescriptor.TraitKey

The symbolic font traits.

static let weight: UIFontDescriptor.TraitKey

The numerical value that corresponds to a font face.

static let width: UIFontDescriptor.TraitKey

The inter-glyph spacing of the font.

