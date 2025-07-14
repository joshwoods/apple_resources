

- Device Management
-  SetAutoAdminPasswordCommand 

Device Management Command

# SetAutoAdminPasswordCommand

The command to change the password of a local administrator account that Setup Assistant creates on a device.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object SetAutoAdminPasswordCommand
```

## Properties

`Command`

SetAutoAdminPasswordCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Discussion

## Topics

### Commands

object SetAutoAdminPasswordCommand.Command

The request dictionary to change the password of a local administrator account.

## See Also

### Command and Response

object SetAutoAdminPasswordResponse

A response from the device after it processes the command to update the local administrator account password.

