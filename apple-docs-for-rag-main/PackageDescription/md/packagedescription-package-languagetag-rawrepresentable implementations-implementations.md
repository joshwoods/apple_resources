

- PackageDescription
- Package
- LanguageTag
-  RawRepresentable Implementations 

API Collection

# RawRepresentable Implementations

## Topics

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var hashValue: Int

The hash value for language tag.

var rawValue: String

The corresponding value of the raw type.

### Instance Methods

func hash(into: inout Hasher)

Hashes the language tag by feeding the item into the given hasher.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

