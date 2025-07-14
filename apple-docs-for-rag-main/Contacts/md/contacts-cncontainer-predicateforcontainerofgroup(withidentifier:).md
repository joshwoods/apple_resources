

- Contacts
- CNContainer
-  predicateForContainerOfGroup(withIdentifier:) 

Type Method

# predicateForContainerOfGroup(withIdentifier:)

Returns a predicate to find the container of the specified group.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForContainerOfGroup(withIdentifier groupIdentifier: String) -> NSPredicate
```

## Parameters 

`groupIdentifier`  

The group identifier to be matched.

## Return Value

A predicate that can be used to fetch a container from CNContactStore.

## See Also

### Generating Search Predicates for Containers

class func predicateForContainerOfContact(withIdentifier: String) -> NSPredicate

Returns a predicate to find the container of the specified contact.

class func predicateForContainers(withIdentifiers: [String]) -> NSPredicate

Returns a predicate to find the containers with the specified identifiers.

