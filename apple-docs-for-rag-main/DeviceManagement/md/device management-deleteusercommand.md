

- Device Management
-  DeleteUserCommand 

Device Management Command

# DeleteUserCommand

The command to delete a user’s account from a device.

iOS 9.3+iPadOS 9.3+macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object DeleteUserCommand
```

## Properties

`Command`

DeleteUserCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Mentioned in 

Handling NotNow Status Responses

## Topics

### Commands

object DeleteUserCommand.Command

The request dictionary to delete a user’s account from a device.

## See Also

### Command and Response

object DeleteUserResponse

A response from the device after it processes the command to delete a user’s account.

