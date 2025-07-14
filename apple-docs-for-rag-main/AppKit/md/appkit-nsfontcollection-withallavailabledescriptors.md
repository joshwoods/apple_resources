

- AppKit
- NSFontCollection
-  withAllAvailableDescriptors 

Type Property

# withAllAvailableDescriptors

The font collection that matches all registered fonts.

macOS 10.7+

``` source
@NSCopying
class var withAllAvailableDescriptors: NSFontCollection { get }
```

## Return Value

The collection of all fonts available to the current application.

## See Also

### Creating Font Collections

init(descriptors: [NSFontDescriptor])

Returns a font collection matching the given descriptors.

init?(locale: Locale)

Returns a collection of fonts matching the given locale.

init?(name: NSFontCollection.Name)

Creates a named font collection object.

init?(name: NSFontCollection.Name, visibility: NSFontCollection.Visibility)

Creates a font collection with the specified name and font visibility.

