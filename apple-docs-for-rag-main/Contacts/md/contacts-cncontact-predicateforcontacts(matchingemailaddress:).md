

- Contacts
- CNContact
-  predicateForContacts(matchingEmailAddress:) 

Type Method

# predicateForContacts(matchingEmailAddress:)

Returns a predicate to find the contacts whose email address matches the specified value.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
class func predicateForContacts(matchingEmailAddress emailAddress: String) -> NSPredicate
```

## Parameters 

`emailAddress`  

The email address to be matched.

## Return Value

A predicate that you can use to fetch contacts from CNContactStore.

## See Also

### Getting Search Predicates

class func predicateForContacts(matchingName: String) -> NSPredicate

Returns a predicate to find the contacts matching the specified name.

class func predicateForContacts(withIdentifiers: [String]) -> NSPredicate

Returns a predicate to find the contacts matching the specified identifiers.

class func predicateForContactsInGroup(withIdentifier: String) -> NSPredicate

Returns a predicate to find the contacts that are members in the specified group.

class func predicateForContactsInContainer(withIdentifier: String) -> NSPredicate

Returns a predicate to find the contacts in the specified container.

class func predicateForContacts(matching: CNPhoneNumber) -> NSPredicate

Returns a predicate to find the contacts whose phone number matches the specified value.

