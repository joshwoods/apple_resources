

- Contacts
- CNContact
-  predicateForContacts(matchingName:) 

Type Method

# predicateForContacts(matchingName:)

Returns a predicate to find the contacts matching the specified name.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForContacts(matchingName name: String) -> NSPredicate
```

## Parameters 

`name`  

The contact name to be matched.

## Return Value

A predicate that you can use to fetch contacts from CNContactStore.

## Discussion

The name can contain any number of words.

## See Also

### Getting Search Predicates

class func predicateForContacts(withIdentifiers: [String]) -> NSPredicate

Returns a predicate to find the contacts matching the specified identifiers.

class func predicateForContactsInGroup(withIdentifier: String) -> NSPredicate

Returns a predicate to find the contacts that are members in the specified group.

class func predicateForContactsInContainer(withIdentifier: String) -> NSPredicate

Returns a predicate to find the contacts in the specified container.

class func predicateForContacts(matching: CNPhoneNumber) -> NSPredicate

Returns a predicate to find the contacts whose phone number matches the specified value.

class func predicateForContacts(matchingEmailAddress: String) -> NSPredicate

Returns a predicate to find the contacts whose email address matches the specified value.

