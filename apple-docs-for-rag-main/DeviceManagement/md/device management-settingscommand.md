

- Device Management
-  SettingsCommand 

Device Management Command

# SettingsCommand

The command to configure settings on a device.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand
```

## Properties

`Command`

SettingsCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Discussion

This command requires the Settings access right.

## Topics

### Commands

object SettingsCommand.Command

The request dictionary to configure settings on a device.

## See Also

### Command and Response

object SettingsResponse

A response from the device after it processes the command to configure settings on a device.

