

- App Intents
-  IntentPerson 

Structure

# IntentPerson

Information that identifies a person participating in an intents-based interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentPerson
```

## Mentioned in 

Adding parameters to an app intent

## Topics

### Creating a contact

init(identifier: IntentPerson.Identifier, name: IntentPerson.Name, handle: IntentPerson.Handle?, aliases: [IntentPerson.Handle], isMe: Bool, image: DisplayRepresentation.Image?)

### Getting the person’s name

var name: IntentPerson.Name

The name of this `IntentPerson`

enum Name

A type that stores name-related information for a person.

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

enum ParameterMode

The type of interface to show when someone chooses a parameter that contains information about a person.

### Getting person-related identifiers

var identifier: IntentPerson.Identifier

enum Identifier

A type that manages a unique identifier for a person.

### Initializers

init(handle: IntentPerson.Handle)

Initializes an `IntentPerson` from a raw handle, like a phone number or an email address. Use this initializer when the value is not linked to a known contact.

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: EmptyResolverSpecification&lt;IntentPerson>

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

InstanceDisplayRepresentable Implementations

TypeDisplayRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomLocalizedStringResourceConvertible
- Decodable
- DisplayRepresentable
- Encodable
- Equatable
- InstanceDisplayRepresentable
- Sendable
- TypeDisplayRepresentable

