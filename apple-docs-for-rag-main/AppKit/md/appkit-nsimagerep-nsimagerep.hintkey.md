

- AppKit
- NSImageRep
-  NSImageRep.HintKey 

Structure

# NSImageRep.HintKey

Constants for the keys to include in a hints dictionary when drawing the image.

macOS

``` source
struct HintKey
```

## Topics

### Hint Keys

static let ctm: NSImageRep.HintKey

A context transform hint.

static let interpolation: NSImageRep.HintKey

An interpolation hint.

static let userInterfaceLayoutDirection: NSImageRep.HintKey

A layout direction hint.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

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

enum LayoutDirection

Constants that describe the layout direction for the image.

