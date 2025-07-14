

- Contacts
- CNContact
-  isUnifiedWithContact(withIdentifier:) 

Instance Method

# isUnifiedWithContact(withIdentifier:)

Returns a Boolean indicating whether the current contact is a unified contact and includes a contact with the specified identifier.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func isUnifiedWithContact(withIdentifier contactIdentifier: String) -> Bool
```

## Parameters 

`contactIdentifier`  

An identifier for an existing contact. If this string is empty, the method returns false.

## Return Value

true if the current contact is a unified contact and if `contactIdentifier` represents one of the contacts that contributes to the unified information; otherwise, false.

## See Also

### Comparing Contacts

class func descriptorForAllComparatorKeys() -> any CNKeyDescriptor

Fetches all the keys required for the contact sort comparator.

class func comparator(forNameSortOrder: CNContactSortOrder) -> Comparator

Returns a comparator to sort contacts with the specified order.

enum CNContactSortOrder

Indicates the sorting order for contacts.

