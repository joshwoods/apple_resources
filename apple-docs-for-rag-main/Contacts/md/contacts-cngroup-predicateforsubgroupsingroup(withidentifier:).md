

- Contacts
- CNGroup
-  predicateForSubgroupsInGroup(withIdentifier:) 

Type Method

# predicateForSubgroupsInGroup(withIdentifier:)

Returns a predicate to find subgroups in the specified parent group.

macOS 10.11+

``` source
class func predicateForSubgroupsInGroup(withIdentifier parentGroupIdentifier: String) -> NSPredicate
```

## Parameters 

`parentGroupIdentifier`  

The parent group to be matched.

## Return Value

A predicate that you can use to fetch subgroup information from CNContactStore.

## See Also

### Generating Search Predicates for Groups

class func predicateForGroups(withIdentifiers: [String]) -> NSPredicate

Returns a predicate to find groups with the specified identifiers.

class func predicateForGroupsInContainer(withIdentifier: String) -> NSPredicate

Returns a predicate to find groups in the specified container.

