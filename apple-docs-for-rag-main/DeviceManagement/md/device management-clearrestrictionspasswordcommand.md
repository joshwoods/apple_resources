

- Device Management
-  ClearRestrictionsPasswordCommand 

Device Management Command

# ClearRestrictionsPasswordCommand

The command to clear the restrictions passcode on a device to disable or edit parental controls.

iOS 8.0+iPadOS 8.0+Device Assignment ServicesVPP License Management

``` source
object ClearRestrictionsPasswordCommand
```

## Properties

`Command`

ClearRestrictionsPasswordCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object ClearRestrictionsPasswordCommand.Command

The request dictionary to clear a restrictions passcode.

## See Also

### Command and Response

object ClearRestrictionsPasswordResponse

A response from the device after it processes the command to clear the restrictions password and the restrictions on a device.

