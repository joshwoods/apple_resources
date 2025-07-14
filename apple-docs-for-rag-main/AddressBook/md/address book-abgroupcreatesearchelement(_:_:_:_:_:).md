

- Address Book
-  ABGroupCreateSearchElement(\_:\_:\_:\_:\_:) 

Function

# ABGroupCreateSearchElement(\_:\_:\_:\_:\_:)

Creates an ABSearchElement object that specifies a queryfor ABGroup records.

macOS

``` source
func ABGroupCreateSearchElement(
    _ property: CFString!,
    _ label: CFString!,
    _ key: CFString!,
    _ value: CFTypeRef!,
    _ comparison: ABSearchComparison
) -> Unmanaged!
```

## Parameters 

`property`  

The name of the property to search on. It cannot be `NULL`. For a full list of the properties, see `Group Properties` and Common Properties.

`label`  

The label name for a multi-value list. If `property` does not have multiple values, pass `NULL`. If `property` does have multiple values, pass `NULL` to search all the values. By default, ABGroup records don’t contain any multi-value list properties.

`key`  

The key name for a dictionary. If `property` is not a dictionary, pass `NULL`. If `property` is a dictionary, pass `NULL` to search all keys. By default, ABGroup records don’t contain any properties that are dictionaries.

`value`  

The value you are searching for. It cannot be `NULL`

`comparison`  

Specifies the type of comparison to perform, such as kABEqual or kABPrefixMatchCaseInsensitive. For a full list, see ABSearchComparison.

## Return Value

A search element objectthat specifies a query according to the above parameters. You areresponsible for releasing this object.

## Discussion

Use the ABAddressBook ABCopyArrayOfMatchingRecords(_:_:) functionto actually perform the query. Also, see `ABSearchElement C` formore functions that create compound queries.

## See Also

### Groups

func ABCopyArrayOfAllGroups(ABAddressBookRef!) -> Unmanaged&lt;CFArray>!

Returns an array of all the groups in the Address Book database.

func ABGroupAddGroup(ABGroupRef!, ABGroupRef!) -> Bool

Adds a subgroup to another group.

func ABGroupAddMember(ABRecord!, ABRecord!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Adds a person to a group.

Deprecated

func ABGroupCopyArrayOfAllMembers(ABRecord!) -> Unmanaged&lt;CFArray>!

Returns an array of persons in a group.

Deprecated

func ABGroupCopyArrayOfAllSubgroups(ABGroupRef!) -> Unmanaged&lt;CFArray>!

Returns an array containing a group’s subgroups.

func ABGroupCopyDistributionIdentifier(ABGroupRef!, ABPersonRef!, CFString!) -> Unmanaged&lt;CFString>!

Returns the distribution identifier for the given propertyand person.

func ABGroupCopyParentGroups(ABGroupRef!) -> Unmanaged&lt;CFArray>!

Returns an array containing a group’s parents—thegroups that a group belongs to.

func ABGroupCreate() -> Unmanaged&lt;ABRecord>!

Returns a new ABGroup object.

Deprecated

func ABGroupRemoveGroup(ABGroupRef!, ABGroupRef!) -> Bool

Removes a subgroup from a group.

func ABGroupRemoveMember(ABRecord!, ABRecord!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a person from a group.

Deprecated

func ABGroupSetDistributionIdentifier(ABGroupRef!, ABPersonRef!, CFString!, CFString!) -> Bool

Assigning a specific distribution identifier for a person’smulti-value list property so that the group can be used as a distributionlist (mailing list, in the case of an email property).

