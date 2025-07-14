

- Device Management
-  SetRecoveryLockCommand 

Device Management Command

# SetRecoveryLockCommand

The command to set the password for Recovery Lock.

macOS 11.5+Device Assignment ServicesVPP License Management

``` source
object SetRecoveryLockCommand
```

## Properties

`Command`

SetRecoveryLockCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object SetRecoveryLockCommand.Command

The request dictionary to set the Recovery Lock password.

## See Also

### Command and Response

object SetRecoveryLockResponse

A response from the device after it sets the password for Recovery Lock.

