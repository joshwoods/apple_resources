

- AppKit
- NSFontDescriptor
- NSFontDescriptor.FeatureKey
-  selectorIdentifier 

Type Property

# selectorIdentifier

A key that indicates the selector of the font feature.

macOS 10.5+

``` source
static let selectorIdentifier: NSFontDescriptor.FeatureKey
```

## Discussion

The value of this key is an NSNumber object specifying a font feature selector such as common ligature off, traditional character shape, and so on. For more information on Apple Fonts see Fonts for Apple platforms and the AAT Font Feature Registry.

## See Also

### Feature Keys

static let typeIdentifier: NSFontDescriptor.FeatureKey

A key that indicates the type of the font feature.

