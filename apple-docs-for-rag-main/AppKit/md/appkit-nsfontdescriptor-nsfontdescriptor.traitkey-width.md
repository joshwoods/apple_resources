

- AppKit
- NSFontDescriptor
- NSFontDescriptor.TraitKey
-  width 

Type Property

# width

The relative inter-glyph spacing value as a number object.

macOS

``` source
static let width: NSFontDescriptor.TraitKey
```

## Discussion

The value of this key is an NSNumber object. The valid value range is from `-1.0` to `1.0`. The value of `0.0` corresponds to the regular glyph spacing.

## See Also

### Trait Keys

static let symbolic: NSFontDescriptor.TraitKey

The symbolic traits value as a number object.

static let weight: NSFontDescriptor.TraitKey

The normalized weight value as a number object.

static let slant: NSFontDescriptor.TraitKey

The relative slant angle value as a number object.

