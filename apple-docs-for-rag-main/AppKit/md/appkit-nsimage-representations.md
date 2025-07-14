

- AppKit
- NSImage
-  representations 

Instance Property

# representations

An array containing all of the image object’s image representations.

macOS

``` source
var representations: [NSImageRep] { get }
```

## Discussion

This property can contain zero or more NSImageRep objects.

## See Also

### Working with Representations of Images

func addRepresentation(NSImageRep)

Adds the specified image representation object to the image.

func addRepresentations([NSImageRep])

Adds an array of image representation objects to the image.

func removeRepresentation(NSImageRep)

Removes and releases the specified image representation.

func bestRepresentation(for: NSRect, context: NSGraphicsContext?, hints: [NSImageRep.HintKey : Any]?) -> NSImageRep?

Returns the best representation of the image for the specified rectangle using the provided hints.

struct HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

enum LayoutDirection

Constants that describe the layout direction for the image.

