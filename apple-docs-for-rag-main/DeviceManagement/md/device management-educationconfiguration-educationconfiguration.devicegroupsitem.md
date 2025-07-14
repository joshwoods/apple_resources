

- Device Management
- EducationConfiguration
-  EducationConfiguration.DeviceGroupsItem 

Device Management Profile

# EducationConfiguration.DeviceGroupsItem

A device group in the organization.

iOS 9.3+iPadOS 9.3+macOS 10.14+Device Assignment ServicesVPP License Management

``` source
object EducationConfiguration.DeviceGroupsItem
```

## Properties

`Identifier`

`string`

 (Required) 

The unique identifier for the device group in the organization.

`Name`

`string`

 (Required) 

The name of the device group, which must be unique in the organization.

`SerialNumbers`

`[string]`

 (Required) 

The serial numbers of the devices in the group.

## See Also

### Objects

object EducationConfiguration.DepartmentsItem

A department in the organization.

object EducationConfiguration.GroupsItem

An array of dictionaries defining groups.

object EducationConfiguration.UsersItem

A user in the organization.

