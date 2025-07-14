

- Contacts
-  CNContactType 

Enumeration

# CNContactType

The types a contact can be.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
enum CNContactType
```

## Topics

### Constants

case person

The contact is a person.

case organization

The contact is an Organization.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying the Contact

var identifier: String

A value that uniquely identifies a contact on the device.

var contactType: CNContactType

An enum identifying the contact type.

