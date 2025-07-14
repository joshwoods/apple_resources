

- AppKit
- NSFontDescriptor
-  NSFontDescriptor.TraitKey 

Structure

# NSFontDescriptor.TraitKey

Constants that can be used as keys to retrieve information about a font descriptor from its trait dictionary.

macOS

``` source
struct TraitKey
```

## Discussion

These keys are used with traits.

## Topics

### Trait Keys

static let symbolic: NSFontDescriptor.TraitKey

The symbolic traits value as a number object.

static let weight: NSFontDescriptor.TraitKey

The normalized weight value as a number object.

static let width: NSFontDescriptor.TraitKey

The relative inter-glyph spacing value as a number object.

static let slant: NSFontDescriptor.TraitKey

The relative slant angle value as a number object.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Font Traits

var symbolicTraits: NSFontDescriptor.SymbolicTraits

A bit mask that describes the traits of the receiver.

typealias NSFontSymbolicTraits

A symbolic description of stylistic aspects of a font.

