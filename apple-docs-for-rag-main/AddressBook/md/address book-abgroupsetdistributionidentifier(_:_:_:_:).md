

- Address Book
-  ABGroupSetDistributionIdentifier(\_:\_:\_:\_:) 

Function

# ABGroupSetDistributionIdentifier(\_:\_:\_:\_:)

Assigning a specific distribution identifier for a person’smulti-value list property so that the group can be used as a distributionlist (mailing list, in the case of an email property).

macOS

``` source
func ABGroupSetDistributionIdentifier(
    _ group: ABGroupRef!,
    _ person: ABPersonRef!,
    _ property: CFString!,
    _ identifier: CFString!
) -> Bool
```

## Parameters 

`group`  

The group that `person` belongs to.

`person`  

The person whose distribution identifier for `property` you wish to change. If `NULL`, this function raises an exception.

`property`  

The multi-value list property whose distribution identifier you wish to change.

`identifier`  

The new distribution identifier, a label used by a multi-value list such as kABAddressHomeLabel for a kABAddressProperty. Pass `NULL` to reset the distribution identifier to its default, a multi-value list’s primary identifier.

## Return Value

`true` ifsuccessful, `false` otherwise.

## Discussion

The default distribution identifier is a multi-value list’sprimary identifier. Use this function if you need to change thedistribution identifier for a particular person. For example, ifthe default identifier is a person’s home email but you want touse John’s work email, invoke this function passing kABEmailWorkLabel asthe `identifier` parameter, kABEmailProperty asthe `property` parameter, and John’sperson object as the `person` parameter.

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

func ABGroupCreateSearchElement(CFString!, CFString!, CFString!, CFTypeRef!, ABSearchComparison) -> Unmanaged&lt;ABSearchElementRef>!

Creates an ABSearchElement object that specifies a queryfor ABGroup records.

func ABGroupRemoveGroup(ABGroupRef!, ABGroupRef!) -> Bool

Removes a subgroup from a group.

func ABGroupRemoveMember(ABRecord!, ABRecord!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a person from a group.

Deprecated

