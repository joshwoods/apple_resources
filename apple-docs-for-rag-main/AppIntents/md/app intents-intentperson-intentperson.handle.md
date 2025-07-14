

- App Intents
- IntentPerson
-  IntentPerson.Handle 

Structure

# IntentPerson.Handle

A type that describes a single way to contact a person.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Handle
```

## Topics

### Getting the handle label

enum Label

A location description that applies to the handle’s content, for example a work or home phone number.

### Operators

static func == (IntentPerson.Handle, IntentPerson.Handle) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(IntentPerson.Handle.Value, label: IntentPerson.Handle.Label)

init(applicationDefined: String, label: String?)

init(emailAddress: String, label: IntentPerson.Handle.Label)

init(phoneNumber: String, label: IntentPerson.Handle.Label)

### Instance Properties

var hashValue: Int

The hash value.

var label: IntentPerson.Handle.Label

var value: IntentPerson.Handle.Value

The string value for this `Handle`, such as the specific phone number or email address

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum Value

A type that describes the type of contact information in the handle, such as whether it is an email address, or a phone number.

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

### Getting identifying information

var handle: IntentPerson.Handle?

The primary `Handle` used to contact this `IntentPerson`

var aliases: [IntentPerson.Handle]

Other secondary `Handle`s used to contact this `IntentPerson`, if any

var isMe: Bool

Whether this `IntentPerson` represents the owner of the device

var image: DisplayRepresentation.Image?

An image representing this `IntentPerson`

enum ParameterMode

The type of interface to show when someone chooses a parameter that contains information about a person.

