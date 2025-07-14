

- AppKit
- NSImage
-  addRepresentations(\_:) 

Instance Method

# addRepresentations(\_:)

Adds an array of image representation objects to the image.

macOS

``` source
func addRepresentations(_ imageReps: [NSImageRep])
```

## Parameters 

`imageReps`  

An array of `NSImageRep` objects.

## Discussion

After invoking this method, you may need to explicitly set features of the new image representations, such as their size, number of colors, and so on. This is true particularly when the `NSImage` object has multiple image representations to choose from. See NSImageRep and its subclasses for the methods you use to complete initialization.

Representations added by this method are retained by the receiver. Image representations cannot be shared among multiple `NSImage` objects.

## See Also

### Working with Representations of Images

func addRepresentation(NSImageRep)

Adds the specified image representation object to the image.

var representations: [NSImageRep]

An array containing all of the image object’s image representations.

func removeRepresentation(NSImageRep)

Removes and releases the specified image representation.

func bestRepresentation(for: NSRect, context: NSGraphicsContext?, hints: [NSImageRep.HintKey : Any]?) -> NSImageRep?

Returns the best representation of the image for the specified rectangle using the provided hints.

struct HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

enum LayoutDirection

Constants that describe the layout direction for the image.

