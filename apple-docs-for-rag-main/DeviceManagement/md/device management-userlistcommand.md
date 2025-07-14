

- Device Management
-  UserListCommand 

Device Management Command

# UserListCommand

The command to get a list of users with active accounts on a device.

iOS 9.3+iPadOS 9.3+macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object UserListCommand
```

## Properties

`Command`

UserListCommand.Command

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

object UserListCommand.Command

The request dictionary to get a list of users with active accounts on a device.

## See Also

### Command and Response

object UserListResponse

A response from the device after it processes the command to get a list of users with active accounts.

