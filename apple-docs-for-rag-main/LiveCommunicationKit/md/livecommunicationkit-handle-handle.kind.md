

- LiveCommunicationKit
- Handle
-  Handle.Kind 

Enumeration

# Handle.Kind

The type of the handle.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
enum Kind
```

## Topics

### Enumeration Cases

case emailAddress

An email address.

case generic

An unspecified type of handle.

case phoneNumber

A phone number.

### Initializers

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: Int

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
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

