

- AppKit
- NSMutableFontCollection
-  init(name:) 

Initializer

# init(name:)

Creates a mutable named font collection object.

macOS 10.7+

``` source
init?(name: NSFontCollection.Name)
```

## Parameters 

`name`  

The name to apply to the font collection.

## Return Value

A mutable font collection object.

## See Also

### Creating a Font Collection

init(descriptors: [NSFontDescriptor])

Creates a mutable font collection containing the fonts that match the specified font descriptors.

init(locale: Locale)

Creates a mutable font collection containing fonts suitable for the specified locale.

init?(name: NSFontCollection.Name, visibility: NSFontCollection.Visibility)

Creates a mutable font collection with the specified name and font visibility.

class var withAllAvailableDescriptors: NSMutableFontCollection

The mutable font collection that matches all registered fonts.

