

- Contacts
- CNGroup
-  predicateForGroupsInContainer(withIdentifier:) 

Type Method

# predicateForGroupsInContainer(withIdentifier:)

Returns a predicate to find groups in the specified container.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForGroupsInContainer(withIdentifier containerIdentifier: String) -> NSPredicate
```

## Parameters 

`containerIdentifier`  

The container identifier to be matched.

## Return Value

A predicate that you can use to fetch groups from CNContactStore.

## See Also

### Generating Search Predicates for Groups

class func predicateForGroups(withIdentifiers: [String]) -> NSPredicate

Returns a predicate to find groups with the specified identifiers.

class func predicateForSubgroupsInGroup(withIdentifier: String) -> NSPredicate

Returns a predicate to find subgroups in the specified parent group.

