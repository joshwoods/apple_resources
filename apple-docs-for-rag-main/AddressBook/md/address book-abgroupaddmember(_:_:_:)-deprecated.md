

- Address Book
-  ABGroupAddMember(\_:\_:\_:) Deprecated

Function

# ABGroupAddMember(\_:\_:\_:)

Adds a person to a group.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS

**macOS**

``` source
func ABGroupAddMember(
    _ group: ABGroupRef!,
    _ personToAdd: ABPersonRef!
) -> Bool
```

**iOS, iPadOS, Mac Catalyst**

``` source
func ABGroupAddMember(
    _ group: ABRecord!,
    _ person: ABRecord!,
    _ error: UnsafeMutablePointer?>!
) -> Bool
```

Deprecated

use \[CNSaveRequest addMember:toGroup:\]

## Parameters 

`group`  

The group you wish to add `person` to.

`personToAdd`  

The person to add to `group`. If `person` is `NULL`, this function raises an exception.

`person`  

The person to add to `group`. If `person` is `NULL`, this function raises an exception.

## Return Value

`true` ifsuccessful, false otherwise. For example, if `person` isalready in `group`, this function doesnothing but returns `false`.

## See Also

### Groups

func ABCopyArrayOfAllGroups(ABAddressBookRef!) -> Unmanaged&lt;CFArray>!

Returns an array of all the groups in the Address Book database.

func ABGroupAddGroup(ABGroupRef!, ABGroupRef!) -> Bool

Adds a subgroup to another group.

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

