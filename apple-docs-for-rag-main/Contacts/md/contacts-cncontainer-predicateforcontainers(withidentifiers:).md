

- Contacts
- CNContainer
-  predicateForContainers(withIdentifiers:) 

Type Method

# predicateForContainers(withIdentifiers:)

Returns a predicate to find the containers with the specified identifiers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForContainers(withIdentifiers identifiers: [String]) -> NSPredicate
```

## Parameters 

`identifiers`  

The container identifiers to be matched.

## Return Value

A predicate that can be used to fetch containers from CNContactStore.

## See Also

### Generating Search Predicates for Containers

class func predicateForContainerOfContact(withIdentifier: String) -> NSPredicate

Returns a predicate to find the container of the specified contact.

class func predicateForContainerOfGroup(withIdentifier: String) -> NSPredicate

Returns a predicate to find the container of the specified group.

