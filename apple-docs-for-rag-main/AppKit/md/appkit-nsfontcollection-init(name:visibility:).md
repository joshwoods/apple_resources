

- AppKit
- NSFontCollection
-  init(name:visibility:) 

Initializer

# init(name:visibility:)

Creates a font collection with the specified name and font visibility.

macOS 10.7+

``` source
init?(
    name: NSFontCollection.Name,
    visibility: NSFontCollection.Visibility
)
```

## Parameters 

`name`  

The name of the collection.

`visibility`  

The visibility of the collection.

## Return Value

The font collection with the specified name and visibility.

## See Also

### Creating Font Collections

init(descriptors: [NSFontDescriptor])

Returns a font collection matching the given descriptors.

init?(locale: Locale)

Returns a collection of fonts matching the given locale.

init?(name: NSFontCollection.Name)

Creates a named font collection object.

class var withAllAvailableDescriptors: NSFontCollection

The font collection that matches all registered fonts.

