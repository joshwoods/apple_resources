

- AppKit
- NSImage
-  removeRepresentation(\_:) 

Instance Method

# removeRepresentation(\_:)

Removes and releases the specified image representation.

macOS

``` source
func removeRepresentation(_ imageRep: NSImageRep)
```

## Parameters 

`imageRep`  

The image representation object you want to remove.

## See Also

### Working with Representations of Images

func addRepresentation(NSImageRep)

Adds the specified image representation object to the image.

func addRepresentations([NSImageRep])

Adds an array of image representation objects to the image.

var representations: [NSImageRep]

An array containing all of the image object’s image representations.

func bestRepresentation(for: NSRect, context: NSGraphicsContext?, hints: [NSImageRep.HintKey : Any]?) -> NSImageRep?

Returns the best representation of the image for the specified rectangle using the provided hints.

struct HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

enum LayoutDirection

Constants that describe the layout direction for the image.

