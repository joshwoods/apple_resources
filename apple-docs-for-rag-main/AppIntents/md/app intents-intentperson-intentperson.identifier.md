

- App Intents
- IntentPerson
-  IntentPerson.Identifier 

Enumeration

# IntentPerson.Identifier

A type that manages a unique identifier for a person.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Identifier
```

## Topics

### Getting the identifier types

case contact(String)

An identifier from the Contacts framework (see `CNContact.identifier`)

case applicationDefined(String)

An identifier specific to your app

### Operators

static func == (IntentPerson.Identifier, IntentPerson.Identifier) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case unknown

Unknown identifier, as in the case where the `IntentPerson` simply wraps a `Handle`.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Getting person-related identifiers

var identifier: IntentPerson.Identifier

