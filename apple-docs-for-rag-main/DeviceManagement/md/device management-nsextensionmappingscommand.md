

- Device Management
-  NSExtensionMappingsCommand 

Device Management Command

# NSExtensionMappingsCommand

The command to get a list of the installed extensions for a user on a device.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object NSExtensionMappingsCommand
```

## Properties

`Command`

NSExtensionMappingsCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object NSExtensionMappingsCommand.Command

The request dictionary to get a list of the installed extensions for a user on a device.

## See Also

### Command and Response

object NSExtensionMappingsResponse

A response from the device after it processes the command to get a list of the installed extensions for a user.

