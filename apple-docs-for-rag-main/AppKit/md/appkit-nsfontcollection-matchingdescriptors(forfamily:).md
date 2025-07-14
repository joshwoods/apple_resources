

- AppKit
- NSFontCollection
-  matchingDescriptors(forFamily:) 

Instance Method

# matchingDescriptors(forFamily:)

Returns an array of font descriptors matching the logical descriptors for the given font family.

macOS 10.7+

``` source
func matchingDescriptors(forFamily family: String) -> [NSFontDescriptor]?
```

## Parameters 

`family`  

The font family whose descriptors are matched.

## Return Value

The matchingDescriptors for the given family.

## See Also

### Getting the Font Descriptors

var matchingDescriptors: [NSFontDescriptor]?

An array of font descriptors matching the logical descriptors.

func matchingDescriptors(forFamily: String, options: [NSFontCollectionMatchingOptionKey : NSNumber]?) -> [NSFontDescriptor]?

Returns an array of font descriptors matching the logical descriptors for the given font family and options.

func matchingDescriptors(options: [NSFontCollectionMatchingOptionKey : NSNumber]?) -> [NSFontDescriptor]?

Returns an array of font descriptors matching the logical descriptors with the given options.

struct NSFontCollectionMatchingOptionKey

These constants are used by the matchingDescriptors(options:) and matchingDescriptors(forFamily:options:) options dictionary parameters.

var queryDescriptors: [NSFontDescriptor]?

An array of font descriptors whose matching results produce the collection’s matching descriptors.

var exclusionDescriptors: [NSFontDescriptor]?

A list of query font descriptors whose matching results are excluded from the list of matching descriptors.

