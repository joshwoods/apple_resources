

- Device Management
-  LOMSetupRequestCommand 

Device Management Command

# LOMSetupRequestCommand

The command to get information from a device to set up lights-out management (LOM).

macOS 11.0+Device Assignment ServicesVPP License Management

``` source
object LOMSetupRequestCommand
```

## Properties

`Command`

LOMSetupRequestCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object LOMSetupRequestCommand.Command

The request dictionary to get information from a device to set up lights-out management (LOM).

## See Also

### Command and Response

object LOMSetupRequestResponse

A response from the device after it processes the command to get setup information for lights-out management (LOM).

