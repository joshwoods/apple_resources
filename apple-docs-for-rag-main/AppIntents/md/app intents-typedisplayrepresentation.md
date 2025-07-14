

- App Intents
-  TypeDisplayRepresentation 

Structure

# TypeDisplayRepresentation

A type that describes the user interface presentation of a custom type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct TypeDisplayRepresentation
```

## Topics

### Initializers

init(name: LocalizedStringResource, numericFormat: LocalizedStringResource?)

init(name: LocalizedStringResource, numericFormat: LocalizedStringResource?, synonyms: [LocalizedStringResource])

init(stringLiteral: String)

Creates an instance initialized to the given string value.

### Instance Properties

var name: LocalizedStringResource

The singular type name, e.g. “Book”.

var numericFormat: LocalizedStringResource?

A string representing a count for the type, e.g. “2 books”.

var synonyms: [LocalizedStringResource]

A list of localized phrases that are synonyms of this particular type display representation

### Type Aliases

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias StringLiteralType

A type that represents a string literal.

typealias UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

### Default Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

## Relationships

### Conforms To

- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Sendable

## See Also

### Entity presentation

struct DisplayRepresentation

A type that describes the user interface presentation of a custom type.

protocol DisplayRepresentable

An interface for providing a dynamic visual representation of a specific type and instances of that type.

protocol InstanceDisplayRepresentable

An interface for providing the visual representation for an instance of a specific type.

protocol TypeDisplayRepresentable

An interface for providing the visual representation of a specific type.

protocol StaticDisplayRepresentable

An interface for providing a static visual representation of a specific type.

protocol CaseDisplayRepresentable

An interface for providing the visual representation for an iterable collection of values.

