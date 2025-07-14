

- Contacts
- CNGroup
-  predicateForGroups(withIdentifiers:) 

Type Method

# predicateForGroups(withIdentifiers:)

Returns a predicate to find groups with the specified identifiers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForGroups(withIdentifiers identifiers: [String]) -> NSPredicate
```

## Parameters 

`identifiers`  

The group identifiers to be matched.

## Return Value

A predicate that can be used to fetch groups from CNContactStore.

## See Also

### Generating Search Predicates for Groups

class func predicateForGroupsInContainer(withIdentifier: String) -> NSPredicate

Returns a predicate to find groups in the specified container.

class func predicateForSubgroupsInGroup(withIdentifier: String) -> NSPredicate

Returns a predicate to find subgroups in the specified parent group.

