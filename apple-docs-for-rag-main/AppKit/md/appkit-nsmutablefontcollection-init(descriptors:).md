

- AppKit
- NSMutableFontCollection
-  init(descriptors:) 

Initializer

# init(descriptors:)

Creates a mutable font collection containing the fonts that match the specified font descriptors.

macOS 10.7+

``` source
init(descriptors queryDescriptors: [NSFontDescriptor])
```

## Parameters 

`queryDescriptors`  

One or more query descriptors describing the fonts to include in the collection.

## Return Value

A mutable font collection object.

## See Also

### Creating a Font Collection

init(locale: Locale)

Creates a mutable font collection containing fonts suitable for the specified locale.

init?(name: NSFontCollection.Name)

Creates a mutable named font collection object.

init?(name: NSFontCollection.Name, visibility: NSFontCollection.Visibility)

Creates a mutable font collection with the specified name and font visibility.

class var withAllAvailableDescriptors: NSMutableFontCollection

The mutable font collection that matches all registered fonts.

