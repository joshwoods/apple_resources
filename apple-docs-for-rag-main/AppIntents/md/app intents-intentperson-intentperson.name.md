

- App Intents
- IntentPerson
-  IntentPerson.Name 

Enumeration

# IntentPerson.Name

A type that stores name-related information for a person.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Name
```

## Topics

### Getting a displayable name

case displayName(String)

The user-visible display name of this `IntentPerson`.

### Getting the name components

case components(PersonNameComponents)

Structured components of this `IntentPerson`’s name

### Operators

static func == (IntentPerson.Name, IntentPerson.Name) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case unknown

Unknown name, as in the case where the `IntentPerson` simply wraps a `Handle`.

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
- Sendable

## See Also

### Getting the person’s name

var name: IntentPerson.Name

The name of this `IntentPerson`

