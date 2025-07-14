

- Contacts
- CNContact
-  descriptorForAllComparatorKeys() 

Type Method

# descriptorForAllComparatorKeys()

Fetches all the keys required for the contact sort comparator.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func descriptorForAllComparatorKeys() -> any CNKeyDescriptor
```

## Return Value

A descriptor object that defines the keys required by the sort comparator.

## Discussion

Use the returned object to specify the keys you want to fetch from the database. For example, use it when creating a CNContactFetchRequest object.

## See Also

### Comparing Contacts

class func comparator(forNameSortOrder: CNContactSortOrder) -> Comparator

Returns a comparator to sort contacts with the specified order.

func isUnifiedWithContact(withIdentifier: String) -> Bool

Returns a Boolean indicating whether the current contact is a unified contact and includes a contact with the specified identifier.

enum CNContactSortOrder

Indicates the sorting order for contacts.

