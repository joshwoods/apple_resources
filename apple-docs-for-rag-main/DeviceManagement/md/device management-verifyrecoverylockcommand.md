

- Device Management
-  VerifyRecoveryLockCommand 

Device Management Command

# VerifyRecoveryLockCommand

The command to verify the password for Recovery Lock.

macOS 11.5+Device Assignment ServicesVPP License Management

``` source
object VerifyRecoveryLockCommand
```

## Properties

`Command`

VerifyRecoveryLockCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object VerifyRecoveryLockCommand.Command

The request dictionary to verify the Recovery Lock password.

## See Also

### Command and Response

object VerifyRecoveryLockResponse

A response from the device after it verifies the password for Recovery Lock.

