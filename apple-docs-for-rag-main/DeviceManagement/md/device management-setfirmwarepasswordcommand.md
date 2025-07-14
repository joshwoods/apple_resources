

- Device Management
-  SetFirmwarePasswordCommand 

Device Management Command

# SetFirmwarePasswordCommand

The command to change or clear the firmware password on a device.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object SetFirmwarePasswordCommand
```

## Properties

`Command`

SetFirmwarePasswordCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object SetFirmwarePasswordCommand.Command

The request dictionary to change or clear the firmware password.

## See Also

### Command and Response

object SetFirmwarePasswordResponse

A response from the device after it processes the command to set the firmware password.

