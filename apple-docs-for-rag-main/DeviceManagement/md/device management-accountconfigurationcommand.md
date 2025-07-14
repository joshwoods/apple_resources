

- Device Management
-  AccountConfigurationCommand 

Device Management Command

# AccountConfigurationCommand

The command to create a local administrator account on a device.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object AccountConfigurationCommand
```

## Properties

`Command`

AccountConfigurationCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object AccountConfigurationCommand.Command

The request dictionary to create a local administrator account.

## See Also

### Command and Response

object AccountConfigurationResponse

A response from the device after it processes the command to create and configure a local administrator account.

