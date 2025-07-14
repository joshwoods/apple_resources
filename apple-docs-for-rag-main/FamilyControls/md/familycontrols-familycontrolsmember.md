

- FamilyControls
-  FamilyControlsMember 

Enumeration

# FamilyControlsMember

The type of account that Family Controls is currently managing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@objc
enum FamilyControlsMember
```

## Topics

### Enumeration Cases

case child

A value indicating that Family Controls is managing a child account, so that a parent or guardian must enter their authorization credentials.

case individual

A value indicating that Family Controls is managing an individual account, so that the user can enter their authorization credentials.

### Initializers

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var description: String

A nonlocalized description of the type of account, suitable for debugging.

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
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable

