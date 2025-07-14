

- Device Management
-  LogOutUserCommand 

Device Management Command

# LogOutUserCommand

The command to force the current user to log out of a device.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

``` source
object LogOutUserCommand
```

## Properties

`Command`

LogOutUserCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object LogOutUserCommand.Command

The request dictionary to force the current user to log out of a device.

## See Also

### Command and Response

object LogOutUserResponse

A response from the device after it processes the command to force the current user to log out.

