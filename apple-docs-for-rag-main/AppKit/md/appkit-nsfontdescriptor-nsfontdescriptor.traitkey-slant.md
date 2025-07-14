

- AppKit
- NSFontDescriptor
- NSFontDescriptor.TraitKey
-  slant 

Type Property

# slant

The relative slant angle value as a number object.

macOS

``` source
static let slant: NSFontDescriptor.TraitKey
```

## Discussion

The value of this key is an NSNumber object. The valid value range is from `-1.0` to `1.0`. The value of `0.0` corresponds to `0` degree clockwise rotation from the vertical and `1.0` corresponds to `30` degrees clockwise rotation.

## See Also

### Trait Keys

static let symbolic: NSFontDescriptor.TraitKey

The symbolic traits value as a number object.

static let weight: NSFontDescriptor.TraitKey

The normalized weight value as a number object.

static let width: NSFontDescriptor.TraitKey

The relative inter-glyph spacing value as a number object.

