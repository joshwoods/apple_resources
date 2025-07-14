

- Foundation
-  PersonNameComponents 

Structure

# PersonNameComponents

The separate parts of a person’s name, allowing locale-aware formatting.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct PersonNameComponents
```

## Topics

### Creating Person Name Components

init()

Initializes a new person name components structure.

### Accessing Person Name Components

var namePrefix: String?

The portion of a name’s full form of address that precedes the name itself.

var givenName: String?

Name bestowed upon an individual to differentiate them from other members of a group that share a family name.

var middleName: String?

Secondary name bestowed upon an individual to differentiate them from others that have the same given name.

var familyName: String?

Name bestowed upon an individual to denote membership in a group or family.

var nameSuffix: String?

The portion of a name’s full form of address that follows the name itself.

var nickname: String?

Name substituted for the purposes of familiarity.

var phoneticRepresentation: PersonNameComponents?

The phonetic representation name components of the receiver.

### Formatting Person Name Components

func formatted() -> String

Generates a locale-aware string representation of an instance of person name components using the default format style.

func formatted&lt;S>(S) -> S.FormatOutput

Generates a locale-aware string representation of an instance of person name components using the provided format style.

struct FormatStyle

A type used to format a person’s name with a style appropriate for the given locale.

### Using Reference Types

class NSPersonNameComponents

An object that manages the separate parts of a person’s name to allow locale-aware formatting.

### Structures

struct AttributedStyle

struct ParseStrategy

### Initializers

init(String) throws

Creates a person name components object from a given string.

init&lt;S>(S.ParseInput, strategy: S) throws

Creates a person name components object from a given string by applying the provided parsing strategy.

init(namePrefix: String?, givenName: String?, middleName: String?, familyName: String?, nameSuffix: String?, nickname: String?, phoneticRepresentation: PersonNameComponents?)

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- ReferenceConvertible
- Sendable

## See Also

### Names

class PersonNameComponentsFormatter

A formatter that provides localized representations of the components of a person’s name.

