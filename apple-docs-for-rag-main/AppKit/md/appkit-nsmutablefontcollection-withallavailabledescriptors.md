

- AppKit
- NSMutableFontCollection
-  withAllAvailableDescriptors 

Type Property

# withAllAvailableDescriptors

The mutable font collection that matches all registered fonts.

macOS 10.7+

``` source
@NSCopying
class var withAllAvailableDescriptors: NSMutableFontCollection { get }
```

## See Also

### Creating a Font Collection

init(descriptors: [NSFontDescriptor])

Creates a mutable font collection containing the fonts that match the specified font descriptors.

init(locale: Locale)

Creates a mutable font collection containing fonts suitable for the specified locale.

init?(name: NSFontCollection.Name)

Creates a mutable named font collection object.

init?(name: NSFontCollection.Name, visibility: NSFontCollection.Visibility)

Creates a mutable font collection with the specified name and font visibility.

