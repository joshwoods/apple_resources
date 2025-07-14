

- AppKit
- NSImage
-  NSImage.LayoutDirection 

Enumeration

# NSImage.LayoutDirection

Constants that describe the layout direction for the image.

macOS 10.12+

``` source
enum LayoutDirection
```

## Topics

### Layout Directions

case unspecified

An unspecified layout direction.

case leftToRight

A left-to-right layout direction.

case rightToLeft

A right-to-left layout direction.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

func bestRepresentation(for: NSRect, context: NSGraphicsContext?, hints: [NSImageRep.HintKey : Any]?) -> NSImageRep?

Returns the best representation of the image for the specified rectangle using the provided hints.

struct HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

