

- Contacts
- CNContact
-  predicateForContactsInContainer(withIdentifier:) 

Type Method

# predicateForContactsInContainer(withIdentifier:)

Returns a predicate to find the contacts in the specified container.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForContactsInContainer(withIdentifier containerIdentifier: String) -> NSPredicate
```

## Parameters 

`containerIdentifier`  

The container identifier to be matched.

## Return Value

A predicate that can be used to fetch contacts from CNContactStore.

## See Also

### Getting Search Predicates

class func predicateForContacts(matchingName: String) -> NSPredicate

Returns a predicate to find the contacts matching the specified name.

class func predicateForContacts(withIdentifiers: [String]) -> NSPredicate

Returns a predicate to find the contacts matching the specified identifiers.

class func predicateForContactsInGroup(withIdentifier: String) -> NSPredicate

Returns a predicate to find the contacts that are members in the specified group.

class func predicateForContacts(matching: CNPhoneNumber) -> NSPredicate

Returns a predicate to find the contacts whose phone number matches the specified value.

class func predicateForContacts(matchingEmailAddress: String) -> NSPredicate

Returns a predicate to find the contacts whose email address matches the specified value.

