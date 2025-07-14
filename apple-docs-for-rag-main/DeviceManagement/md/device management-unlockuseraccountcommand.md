

- Device Management
-  UnlockUserAccountCommand 

Device Management Command

# UnlockUserAccountCommand

The command to unlock a local user account on a device.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object UnlockUserAccountCommand
```

## Properties

`Command`

UnlockUserAccountCommand.Command

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

object UnlockUserAccountCommand.Command

The request dictionary to unlock a local user account.

## See Also

### Command and Response

object UnlockUserAccountResponse

A response from the device after it processes the command to unlock a user account.

