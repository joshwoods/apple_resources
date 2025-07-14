

- Device Management
-  LOMDeviceRequestCommand 

Device Management Command

# LOMDeviceRequestCommand

The command to send requests to a device using lights-out management (LOM).

macOS 11.0+Device Assignment ServicesVPP License Management

``` source
object LOMDeviceRequestCommand
```

## Properties

`Command`

LOMDeviceRequestCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object LOMDeviceRequestCommand.Command

The request dictionary to send requests to a device using lights-out management (LOM).

## See Also

### Command and Response

object LOMDeviceRequestResponse

A response from the device after it processes requests it receives through lights-out management (LOM).

