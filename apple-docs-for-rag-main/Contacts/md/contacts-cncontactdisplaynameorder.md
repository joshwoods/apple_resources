

- Contacts
-  CNContactDisplayNameOrder 

Enumeration

# CNContactDisplayNameOrder

The formatting orders for contact names component.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
enum CNContactDisplayNameOrder
```

## Topics

### Constants

case userDefault

Display name order by user default.

case givenNameFirst

Display name order by given name first.

case familyNameFirst

Display name order by family name first.

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

### Getting format information

class func delimiter(for: CNContact) -> String

Returns the delimiter to use between name components.

class func nameOrder(for: CNContact) -> CNContactDisplayNameOrder

Returns the display name order.

