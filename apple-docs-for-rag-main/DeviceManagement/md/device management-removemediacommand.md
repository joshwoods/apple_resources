

- Device Management
-  RemoveMediaCommand 

Device Management Command

# RemoveMediaCommand

The command to remove an installed book from a device.

iOS 8.0+iPadOS 8.0+Device Assignment ServicesVPP License Management

``` source
object RemoveMediaCommand
```

## Properties

`Command`

RemoveMediaCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object RemoveMediaCommand.Command

The request dictionary to remove an installed book.

## See Also

### Command and Response

object RemoveMediaResponse

A response from the device after it processes the command to remove a book from a device.

