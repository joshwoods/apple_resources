

- App Intents
- IntentPerson
- IntentPerson.Handle
-  IntentPerson.Handle.Value 

Enumeration

# IntentPerson.Handle.Value

A type that describes the type of contact information in the handle, such as whether it is an email address, or a phone number.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Value
```

## Topics

### Operators

static func == (IntentPerson.Handle.Value, IntentPerson.Handle.Value) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case applicationDefined(String)

An application-defined point of contact, such as a username of an a social networking service

case emailAddress(String)

case phoneNumber(String)

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

