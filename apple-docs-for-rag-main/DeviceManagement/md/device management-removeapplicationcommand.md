

- Device Management
-  RemoveApplicationCommand 

Device Management Command

# RemoveApplicationCommand

The command to remove an installed managed app from a device.

iOS 5.0+iPadOS 5.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object RemoveApplicationCommand
```

## Properties

`Command`

RemoveApplicationCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object RemoveApplicationCommand.Command

The request dictionary to remove an installed managed app.

## See Also

### Command and Response

object RemoveApplicationResponse

A response from the device after it processes the command to remove a managed app.

