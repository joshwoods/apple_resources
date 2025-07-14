

- AppKit
- NSFontCollection
-  init(descriptors:) 

Initializer

# init(descriptors:)

Returns a font collection matching the given descriptors.

macOS 10.7+

``` source
init(descriptors queryDescriptors: [NSFontDescriptor])
```

## Parameters 

`queryDescriptors`  

The descriptors used to match the returned collection.

## Return Value

The font collection matching the given descriptors.

## See Also

### Creating Font Collections

init?(locale: Locale)

Returns a collection of fonts matching the given locale.

init?(name: NSFontCollection.Name)

Creates a named font collection object.

init?(name: NSFontCollection.Name, visibility: NSFontCollection.Visibility)

Creates a font collection with the specified name and font visibility.

class var withAllAvailableDescriptors: NSFontCollection

The font collection that matches all registered fonts.

