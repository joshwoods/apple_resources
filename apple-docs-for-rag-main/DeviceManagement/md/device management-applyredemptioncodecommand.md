

- Device Management
-  ApplyRedemptionCodeCommand 

Device Management Command

# ApplyRedemptionCodeCommand

The command to send a redemption code to complete installation of an app on a device.

iOS 5.0+iPadOS 5.0+Device Assignment ServicesVPP License Management

``` source
object ApplyRedemptionCodeCommand
```

## Properties

`Command`

ApplyRedemptionCodeCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object ApplyRedemptionCodeCommand.Command

The request dictionary to send a redemption code to complete installation of an app.

## See Also

### Command and Response

object ApplyRedemptionCodeResponse

A response from the device after it processes the command to complete the installation of an app using a redemption code.

