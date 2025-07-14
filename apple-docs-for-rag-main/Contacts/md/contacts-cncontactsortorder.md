

- Contacts
-  CNContactSortOrder 

Enumeration

# CNContactSortOrder

Indicates the sorting order for contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
enum CNContactSortOrder
```

## Overview

The value CNContactSortOrder.userDefault is the user’s preferred sort order.

## Topics

### Sort Orders

case none

No sorting order.

case userDefault

The user’s default sorting order.

case givenName

Sorting contacts by given name.

case familyName

Sorting contacts by family name.

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

### Comparing Contacts

class func descriptorForAllComparatorKeys() -> any CNKeyDescriptor

Fetches all the keys required for the contact sort comparator.

class func comparator(forNameSortOrder: CNContactSortOrder) -> Comparator

Returns a comparator to sort contacts with the specified order.

func isUnifiedWithContact(withIdentifier: String) -> Bool

Returns a Boolean indicating whether the current contact is a unified contact and includes a contact with the specified identifier.

