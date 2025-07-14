

- AppKit
- NSMutableFontCollection
-  init(locale:) 

Initializer

# init(locale:)

Creates a mutable font collection containing fonts suitable for the specified locale.

macOS 10.7+

``` source
init(locale: Locale)
```

## Parameters 

`locale`  

The locale associated with the fonts you want.

## Return Value

A mutable collection of fonts matching the specified locale.

## See Also

### Creating a Font Collection

init(descriptors: [NSFontDescriptor])

Creates a mutable font collection containing the fonts that match the specified font descriptors.

init?(name: NSFontCollection.Name)

Creates a mutable named font collection object.

init?(name: NSFontCollection.Name, visibility: NSFontCollection.Visibility)

Creates a mutable font collection with the specified name and font visibility.

class var withAllAvailableDescriptors: NSMutableFontCollection

The mutable font collection that matches all registered fonts.

