

- AppKit
- NSFontCollection
-  init(name:) 

Initializer

# init(name:)

Creates a named font collection object.

macOS 10.7+

``` source
init?(name: NSFontCollection.Name)
```

## Parameters 

`name`  

The name of the collection.

## Return Value

The named font collection.

## See Also

### Creating Font Collections

init(descriptors: [NSFontDescriptor])

Returns a font collection matching the given descriptors.

init?(locale: Locale)

Returns a collection of fonts matching the given locale.

init?(name: NSFontCollection.Name, visibility: NSFontCollection.Visibility)

Creates a font collection with the specified name and font visibility.

class var withAllAvailableDescriptors: NSFontCollection

The font collection that matches all registered fonts.

