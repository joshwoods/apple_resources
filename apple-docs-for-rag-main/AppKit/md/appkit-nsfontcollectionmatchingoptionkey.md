

- AppKit
-  NSFontCollectionMatchingOptionKey 

Structure

# NSFontCollectionMatchingOptionKey

These constants are used by the matchingDescriptors(options:) and matchingDescriptors(forFamily:options:) options dictionary parameters.

macOS

``` source
struct NSFontCollectionMatchingOptionKey
```

## Topics

### Type Properties

static let includeDisabledFontsOption: NSFontCollectionMatchingOptionKey

An NSNumber object containing a Boolean value specifying whether disabled fonts should be included in the list of matching descriptors; true if they should be included, false otherwise. When unspecified, CoreText assumes false. This option is intended only for font management applications. This option will make descriptor matching slower.

static let removeDuplicatesOption: NSFontCollectionMatchingOptionKey

An NSNumber object containing a Boolean value controlling whether more than one copy of a font with the same PostScript name should be included in the list of matching descriptors.

static let disallowAutoActivationOption: NSFontCollectionMatchingOptionKey

An NSNumber object containing a Boolean value specifying that auto-activation should not be used to find missing fonts.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Font Descriptors

var matchingDescriptors: [NSFontDescriptor]?

An array of font descriptors matching the logical descriptors.

func matchingDescriptors(forFamily: String) -> [NSFontDescriptor]?

Returns an array of font descriptors matching the logical descriptors for the given font family.

func matchingDescriptors(forFamily: String, options: [NSFontCollectionMatchingOptionKey : NSNumber]?) -> [NSFontDescriptor]?

Returns an array of font descriptors matching the logical descriptors for the given font family and options.

func matchingDescriptors(options: [NSFontCollectionMatchingOptionKey : NSNumber]?) -> [NSFontDescriptor]?

Returns an array of font descriptors matching the logical descriptors with the given options.

var queryDescriptors: [NSFontDescriptor]?

An array of font descriptors whose matching results produce the collection’s matching descriptors.

var exclusionDescriptors: [NSFontDescriptor]?

A list of query font descriptors whose matching results are excluded from the list of matching descriptors.

