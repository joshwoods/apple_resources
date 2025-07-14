

- AppKit
- NSImage
-  bestRepresentation(for:context:hints:) 

Instance Method

# bestRepresentation(for:context:hints:)

Returns the best representation of the image for the specified rectangle using the provided hints.

macOS 10.6+

``` source
func bestRepresentation(
    for rect: NSRect,
    context referenceContext: NSGraphicsContext?,
    hints: [NSImageRep.HintKey : Any]?
) -> NSImageRep?
```

## Parameters 

`rect`  

The area of the image to return.

`referenceContext`  

A graphics context. This value can be `nil`.

`hints`  

An optional dictionary of hints that provide more context for selecting or generating a `CGImage`, and may override properties of the `referenceContext`. See `Image Hint Dictionary Keys` for a summary of the possible key-value pairs.

## Return Value

The image representation that most closely matches the specified criteria.

## See Also

### Working with Representations of Images

func addRepresentation(NSImageRep)

Adds the specified image representation object to the image.

func addRepresentations([NSImageRep])

Adds an array of image representation objects to the image.

var representations: [NSImageRep]

An array containing all of the image object’s image representations.

func removeRepresentation(NSImageRep)

Removes and releases the specified image representation.

struct HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

enum LayoutDirection

Constants that describe the layout direction for the image.

