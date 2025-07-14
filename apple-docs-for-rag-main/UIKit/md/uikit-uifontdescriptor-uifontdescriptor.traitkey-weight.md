

- UIKit
- UIFontDescriptor
- UIFontDescriptor.TraitKey
-  weight 

Type Property

# weight

The numerical value that corresponds to a font face.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
static let weight: UIFontDescriptor.TraitKey
```

## Discussion

The value of this key is an NSNumber object. The valid value range is from `-1.0` to `1.0`, where `0.0` corresponds to the regular weight constant. The negative side of the value range indicates that the font is light or thin; the positive side means the font is heavier or bolder. For example, the font face ultraLight has the approximate value of `-0.8`, and black has the approximate value of `0.62`. When providing a weight that doesn’t precisely match a font face in the family, the system locates an available face that represents the closest match.

You can use a font face constant to specify a weight; for a list of constants, see UIFont.Weight.

To access the weight of a font, first retrieve the font’s traits dictionary information:

```
let font = UIFont.systemFont(ofSize: 21, weight: .bold)
if let traits = font.fontDescriptor.object(forKey: .traits) as? [UIFontDescriptor.TraitKey: Any]{
    let weightValue = traits[.weight]
}
```

## See Also

### Font traits

static let slant: UIFontDescriptor.TraitKey

The relative slant angle of the font.

static let symbolic: UIFontDescriptor.TraitKey

The symbolic font traits.

static let width: UIFontDescriptor.TraitKey

The inter-glyph spacing of the font.

