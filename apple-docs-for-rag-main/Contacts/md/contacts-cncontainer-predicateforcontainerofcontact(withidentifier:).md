

- Contacts
- CNContainer
-  predicateForContainerOfContact(withIdentifier:) 

Type Method

# predicateForContainerOfContact(withIdentifier:)

Returns a predicate to find the container of the specified contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForContainerOfContact(withIdentifier contactIdentifier: String) -> NSPredicate
```

## Parameters 

`contactIdentifier`  

The contact identifier to be matched.

## Return Value

A predicate that can be used to fetch a container from CNContactStore.

## Discussion

If the identifier is for a unified contact then this method returns an empty array. To fetch the containers of a unified contact, first fetch the linked contacts and then fetch the container of each linked contact.

## See Also

### Generating Search Predicates for Containers

class func predicateForContainers(withIdentifiers: [String]) -> NSPredicate

Returns a predicate to find the containers with the specified identifiers.

class func predicateForContainerOfGroup(withIdentifier: String) -> NSPredicate

Returns a predicate to find the container of the specified group.

