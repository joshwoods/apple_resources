

- AppKit
- NSFontCollection
-  init(locale:) 

Initializer

# init(locale:)

Returns a collection of fonts matching the given locale.

macOS 10.7+

``` source
init?(locale: Locale)
```

## Parameters 

`locale`  

The locale to match.

## Return Value

A collection of fonts matching the given locale.

## See Also

### Creating Font Collections

init(descriptors: [NSFontDescriptor])

Returns a font collection matching the given descriptors.

init?(name: NSFontCollection.Name)

Creates a named font collection object.

init?(name: NSFontCollection.Name, visibility: NSFontCollection.Visibility)

Creates a font collection with the specified name and font visibility.

class var withAllAvailableDescriptors: NSFontCollection

The font collection that matches all registered fonts.

