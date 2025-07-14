

- Device Management
- SettingsCommand
-  SettingsCommand.Command 

Device Management Command

# SettingsCommand.Command

The request dictionary to configure settings on a device.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to configure settings on a device.

Value: `Settings`

`Settings`

SettingsCommand.Command.Settings

 (Required) 

An array of dictionaries that contains the settings.

## Topics

### Commands

object SettingsCommand.Command.Settings

An array of dictionaries that contains the settings.

