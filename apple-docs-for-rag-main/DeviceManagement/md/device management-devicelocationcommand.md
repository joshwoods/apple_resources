

- Device Management
-  DeviceLocationCommand 

Device Management Command

# DeviceLocationCommand

The command to request a device’s location.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

``` source
object DeviceLocationCommand
```

## Properties

`Command`

DeviceLocationCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object DeviceLocationCommand.Command

The request dictionary to request a device’s location.

## See Also

### Command and Response

object DeviceLocationResponse

A response from a device in Lost Mode after it processes the command to request its location.

