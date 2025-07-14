

- AppKit
- NSGraphicsContext
-  NSGraphicsContext.AttributeKey 

Structure

# NSGraphicsContext.AttributeKey

Constants that specify the dictionary keys for the attributes of the graphics context.

macOS

``` source
struct AttributeKey
```

## Discussion

You use these dictionary keys with init(attributes:) and attributes.

## Topics

### Attribute Keys

static let destination: NSGraphicsContext.AttributeKey

Specifies the destination.

static let representationFormat: NSGraphicsContext.AttributeKey

Specifies the destination file format.

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

struct RepresentationFormatName

Constants that specify values for the representation format name key in a graphic context’s attributes dictionary.

var isFlipped: Bool

A Boolean value that indicates the graphics context’s flipped state.

