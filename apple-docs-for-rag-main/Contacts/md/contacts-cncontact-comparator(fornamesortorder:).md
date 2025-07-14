

- Contacts
- CNContact
-  comparator(forNameSortOrder:) 

Type Method

# comparator(forNameSortOrder:)

Returns a comparator to sort contacts with the specified order.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func comparator(forNameSortOrder sortOrder: CNContactSortOrder) -> Comparator
```

## Parameters 

`sortOrder`  

The preferred sort order, such as by given name.

## Return Value

A comparator to order contacts.

## See Also

### Comparing Contacts

class func descriptorForAllComparatorKeys() -> any CNKeyDescriptor

Fetches all the keys required for the contact sort comparator.

func isUnifiedWithContact(withIdentifier: String) -> Bool

Returns a Boolean indicating whether the current contact is a unified contact and includes a contact with the specified identifier.

enum CNContactSortOrder

Indicates the sorting order for contacts.

