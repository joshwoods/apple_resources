

- AppKit
- NSFontCollectionMatchingOptionKey
-  removeDuplicatesOption 

Type Property

# removeDuplicatesOption

An NSNumber object containing a Boolean value controlling whether more than one copy of a font with the same PostScript name should be included in the list of matching descriptors.

macOS 10.7+

``` source
static let removeDuplicatesOption: NSFontCollectionMatchingOptionKey
```

## See Also

### Type Properties

static let includeDisabledFontsOption: NSFontCollectionMatchingOptionKey

An NSNumber object containing a Boolean value specifying whether disabled fonts should be included in the list of matching descriptors; true if they should be included, false otherwise. When unspecified, CoreText assumes false. This option is intended only for font management applications. This option will make descriptor matching slower.

static let disallowAutoActivationOption: NSFontCollectionMatchingOptionKey

An NSNumber object containing a Boolean value specifying that auto-activation should not be used to find missing fonts.

