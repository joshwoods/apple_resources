

- App Intents
- IntentPerson
-  IntentPerson.ParameterMode 

Enumeration

# IntentPerson.ParameterMode

The type of interface to show when someone chooses a parameter that contains information about a person.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum ParameterMode
```

## Topics

### Getting the interface type

case contact

The parameter shows an interface allowing the user to pick a contact

case email

The parameter shows an interface allowing the user to pick an email

case emailOrPhone

The parameter shows an interface allowing the user to pick an email or phone number

case phone

The parameter shows an interface allowing the user to pick a phone number

### Creating a parameter mode

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Getting identifying information

var handle: IntentPerson.Handle?

The primary `Handle` used to contact this `IntentPerson`

var aliases: [IntentPerson.Handle]

Other secondary `Handle`s used to contact this `IntentPerson`, if any

var isMe: Bool

Whether this `IntentPerson` represents the owner of the device

var image: DisplayRepresentation.Image?

An image representing this `IntentPerson`

struct Handle

A type that describes a single way to contact a person.

