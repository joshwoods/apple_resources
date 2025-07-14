

- AppKit
- NSMutableFontCollection
-  init(name:visibility:) 

Initializer

# init(name:visibility:)

Creates a mutable font collection with the specified name and font visibility.

macOS 10.7+

``` source
init?(
    name: NSFontCollection.Name,
    visibility: NSFontCollection.Visibility
)
```

## Parameters 

`name`  

The name to apply to the font collection.

`visibility`  

The visibility of the fonts in the collection.

## Return Value

A mutable font collection object.

## See Also

### Creating a Font Collection

init(descriptors: [NSFontDescriptor])

Creates a mutable font collection containing the fonts that match the specified font descriptors.

init(locale: Locale)

Creates a mutable font collection containing fonts suitable for the specified locale.

init?(name: NSFontCollection.Name)

Creates a mutable named font collection object.

class var withAllAvailableDescriptors: NSMutableFontCollection

The mutable font collection that matches all registered fonts.

