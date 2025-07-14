

- Address Book
-  ABGroupCopyDistributionIdentifier(\_:\_:\_:) 

Function

# ABGroupCopyDistributionIdentifier(\_:\_:\_:)

Returns the distribution identifier for the given propertyand person.

macOS

``` source
func ABGroupCopyDistributionIdentifier(
    _ group: ABGroupRef!,
    _ person: ABPersonRef!,
    _ property: CFString!
) -> Unmanaged!
```

## Parameters 

`group`  

The group object that `person` belongs to.

`person`  

A person object whose distribution identifier you want to obtain.

`property`  

The name of a person’s multi-value list property whose distribution identifier you want to obtain.

## Return Value

The distribution identifierfor `person` and `property` ifit was set, otherwise returns the property’s primary identifier.If either `person` or `property` are `NULL`,this function returns `NULL`. Also,returns `NULL` if `property` isnot a multi-value list property. You are responsible for releasingthis object.

## Discussion

Use the ABGroupSetDistributionIdentifier(_:_:_:_:) functionto set the distribution identifier for a person’s multi-valuelist property.

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

func ABGroupCopyParentGroups(ABGroupRef!) -> Unmanaged&lt;CFArray>!

Returns an array containing a group’s parents—thegroups that a group belongs to.

func ABGroupCreate() -> Unmanaged&lt;ABRecord>!

Returns a new ABGroup object.

Deprecated

func ABGroupCreateSearchElement(CFString!, CFString!, CFString!, CFTypeRef!, ABSearchComparison) -> Unmanaged&lt;ABSearchElementRef>!

Creates an ABSearchElement object that specifies a queryfor ABGroup records.

func ABGroupRemoveGroup(ABGroupRef!, ABGroupRef!) -> Bool

Removes a subgroup from a group.

func ABGroupRemoveMember(ABRecord!, ABRecord!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a person from a group.

Deprecated

func ABGroupSetDistributionIdentifier(ABGroupRef!, ABPersonRef!, CFString!, CFString!) -> Bool

Assigning a specific distribution identifier for a person’smulti-value list property so that the group can be used as a distributionlist (mailing list, in the case of an email property).

