

- Device Management
-  Device 

Object

# Device

A device’s properties and their values.

Device Assignment ServicesVPP License Management

``` source
object Device
```

## Properties

`asset_tag`

`string`

The device’s asset tag.

`color`

`string`

The color of the device.

`description`

`string`

A description of the device.

`device_assigned_by`

`string`

The email of the person who assigned the device.

`device_assigned_date`

`string`

A time stamp in ISO 8601 format that indicates when the device was assigned to the MDM server.

`device_family`

`string`

The device’s Apple product family: `iPad`, `iPhone`, `iPod`, `Mac`, `AppleTV`, or `Vision`. This key is valid in X-Server-Protocol-Version 2 and later.

`model`

`string`

The model name.

`op_date`

`string`

A time stamp in ISO 8601 format that indicates when the device was added, updated, or deleted. If the value of `op_type` is added, this is the same as `device_assigned_date`. This field is only applicable with the Sync the List of Devices command.

`op_type`

`string`

Indicates whether the device was added (assigned to the MDM server), modified, or deleted. Contains one of the following strings: `added`, `modified`, or `deleted.This` field is only applicable with the `sync the list of devices` command.

`os`

`string`

The device’s operating system: `iOS`, `iPadOS`, `OSX`, `tvOS`, or `visionOS`.

This key is valid in X-Server-Protocol-Version 2 and later.

With X-Server-Protocol-Version 7 and later, iPad product os will return `iPadOS`.

`profile_assign_time`

`string`

A time stamp in ISO 8601 format that indicates when a profile was assigned to the device.

`profile_push_time`

`string`

A time stamp in ISO 8601 format that indicates when a profile was pushed to the device.

`profile_status`

`string`

The status of profile installation—either `empty`, `assigned`, `pushed`, or `removed`.

`profile_uuid`

`string`

The unique ID of the assigned profile.

`serial_number`

`string`

The device’s serial number.

## See Also

### Objects and Data Types

object MachineInfo

A device’s information in response to a MDM enrollment profile request.

object Profile

A profile’s properties and their values.

object Limit

A ranged limit.

object Url

A URL object.

