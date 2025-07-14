

- Device Management
-  InstallApplicationCommand 

Device Management Command

# InstallApplicationCommand

The command to install an app on a device.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstallApplicationCommand
```

## Properties

`Command`

InstallApplicationCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object InstallApplicationCommand.Command

The request dictionary to install an app.

## See Also

### Command and Response

object InstallApplicationResponse

A response from the device after it processes the command to install a third-party app.

