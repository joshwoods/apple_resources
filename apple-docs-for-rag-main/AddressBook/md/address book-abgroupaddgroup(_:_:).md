

- Address Book
-  ABGroupAddGroup(\_:\_:) 

Function

# ABGroupAddGroup(\_:\_:)

Adds a subgroup to another group.

macOS

``` source
func ABGroupAddGroup(
    _ group: ABGroupRef!,
    _ groupToAdd: ABGroupRef!
) -> Bool
```

## Parameters 

`group`  

The group you wish to add a subgroup to. If `NULL`, this function raises an exception.

`groupToAdd`  

The subgroup you wish to add to `group`.

## Return Value

Returns `true` ifsuccessful. If the `group` argumentis already part of the receiver, this function does nothing andreturns `false`. If adding the group wouldcreate a recursion, this function also does nothing and returns `false`. Forexample, if the group “Animal Lovers” is in “Dog Lovers,“and you add “Dog Lovers” to “Animal Lovers,” that wouldcreate a recursion, which this function won’t allow.

## See Also

### Groups

func ABCopyArrayOfAllGroups(ABAddressBookRef!) -> Unmanaged&lt;CFArray>!

Returns an array of all the groups in the Address Book database.

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

func ABGroupSetDistributionIdentifier(ABGroupRef!, ABPersonRef!, CFString!, CFString!) -> Bool

Assigning a specific distribution identifier for a person’smulti-value list property so that the group can be used as a distributionlist (mailing list, in the case of an email property).

