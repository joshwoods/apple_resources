

- Device Management
- EducationConfiguration
-  EducationConfiguration.GroupsItem 

Device Management Profile

# EducationConfiguration.GroupsItem

An array of dictionaries defining groups.

iOS 9.3+iPadOS 9.3+macOS 10.14+Device Assignment ServicesVPP License Management

``` source
object EducationConfiguration.GroupsItem
```

## Properties

`BeaconID`

`integer`

 (Required) 

An unsigned 16 bit integer specifying this group’s unique beacon ID.

`ConfigurationSource`

`string`

The source that provided this group, such as iTunesU, SIS, or MDM.

`Description`

`string`

The description of the group.

`DeviceGroupIdentifiers`

`[string]`

The identifiers that refer to entries in the `DeviceGroups` array to which the instructor can assign users from this class.

Has no effect on the configuration of the Shared iPad login screen.

`ImageURL`

`string`

Deprecated 

Deprecated in iOS 9.3.1 and later. The URL of an image for the group.

`LeaderIdentifiers`

`[string]`

The user identifiers that are leaders of this group.

`MemberIdentifiers`

`[string]`

 (Required) 

The entries in the Users array that are members of the group.

`Name`

`string`

 (Required) 

The display name of the group.

## Discussion

*For shared iPads:* An array of dictionaries that define groups that the user can select in the login window.

*For leader/teacher profiles:* An array of dictionaries that define the groups that the user can control.

## See Also

### Objects

object EducationConfiguration.DepartmentsItem

A department in the organization.

object EducationConfiguration.DeviceGroupsItem

A device group in the organization.

object EducationConfiguration.UsersItem

A user in the organization.

