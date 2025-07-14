

- Address Book
-  ABGroupRemoveMember(\_:\_:\_:) Deprecated

Function

# ABGroupRemoveMember(\_:\_:\_:)

Removes a person from a group.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS

**macOS**

``` source
func ABGroupRemoveMember(
    _ group: ABGroupRef!,
    _ personToRemove: ABPersonRef!
) -> Bool
```

**iOS, iPadOS, Mac Catalyst**

``` source
func ABGroupRemoveMember(
    _ group: ABRecord!,
    _ member: ABRecord!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

Deprecated

use \[CNSaveRequest removeMember:fromGroup:\]

## Parameters 

`group`  

The group that you wish to remove `person` from.

`personToRemove`  

The member that you wish to remove from `group`.

`member`  

The person that you wish to remove from group.

## Return Value

`true` ifsuccessful. If the `person` parameteris not in `group`, this function does nothingand returns `false`.

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

func ABGroupSetDistributionIdentifier(ABGroupRef!, ABPersonRef!, CFString!, CFString!) -> Bool

Assigning a specific distribution identifier for a person’smulti-value list property so that the group can be used as a distributionlist (mailing list, in the case of an email property).

