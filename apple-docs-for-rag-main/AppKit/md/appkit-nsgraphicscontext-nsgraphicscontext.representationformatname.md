

- AppKit
- NSGraphicsContext
-  NSGraphicsContext.RepresentationFormatName 

Structure

# NSGraphicsContext.RepresentationFormatName

Constants that specify values for the representation format name key in a graphic context’s attributes dictionary.

macOS

``` source
struct RepresentationFormatName
```

## Discussion

You use these constants with the representationFormat key.

## Topics

### Format Names

static let pdf: NSGraphicsContext.RepresentationFormatName

Destination file format is PDF.

static let postScript: NSGraphicsContext.RepresentationFormatName

Destination file format is PostScript.

### Initializers

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Information About the Context

var attributes: [NSGraphicsContext.AttributeKey : Any]?

The attributes used to create this instance.

struct AttributeKey

Constants that specify the dictionary keys for the attributes of the graphics context.

var isFlipped: Bool

A Boolean value that indicates the graphics context’s flipped state.

