

- Device Management
- ScheduleOSUpdateCommand
-  ScheduleOSUpdateCommand.Command 

Device Management Command

# ScheduleOSUpdateCommand.Command

The request dictionary to schedule an update of the operating system.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 12.0+Device Assignment ServicesVPP License Management

``` source
object ScheduleOSUpdateCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to schedule an update of the operating system.

Value: `ScheduleOSUpdate`

`Updates`

`[`ScheduleOSUpdateCommand.Command.UpdatesItem`]`

 (Required) 

An array of dictionaries specifying the updates to download or install. If this value is missing, the device applies the default behavior for handling updates.

## Topics

### Commands

object ScheduleOSUpdateCommand.Command.UpdatesItem

A dictionary that describes the available operating-system updates item.

