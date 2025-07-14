

- App Intents
-  DisplayRepresentation 

Structure

# DisplayRepresentation

A type that describes the user interface presentation of a custom type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct DisplayRepresentation
```

## Mentioned in 

Integrating custom data types into your intents

## Topics

### Creating a representation

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(title: LocalizedStringResource, subtitle: LocalizedStringResource?, image: DisplayRepresentation.Image?)

### Displaying the content

var title: LocalizedStringResource

var subtitle: LocalizedStringResource?

var image: DisplayRepresentation.Image?

struct Image

### Operators

static func == (DisplayRepresentation, DisplayRepresentation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(title: LocalizedStringResource, subtitle: LocalizedStringResource?, image: DisplayRepresentation.Image?, synonyms: [LocalizedStringResource])

### Instance Properties

var synonyms: [LocalizedStringResource]

A list of localized phrases that are synonyms of this particular display representation

### Type Aliases

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias StringLiteralType

A type that represents a string literal.

typealias UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

### Default Implementations

Equatable Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Sendable

## See Also

### Entity presentation

protocol DisplayRepresentable

An interface for providing a dynamic visual representation of a specific type and instances of that type.

protocol InstanceDisplayRepresentable

An interface for providing the visual representation for an instance of a specific type.

protocol TypeDisplayRepresentable

An interface for providing the visual representation of a specific type.

struct TypeDisplayRepresentation

A type that describes the user interface presentation of a custom type.

protocol StaticDisplayRepresentable

An interface for providing a static visual representation of a specific type.

protocol CaseDisplayRepresentable

An interface for providing the visual representation for an iterable collection of values.

