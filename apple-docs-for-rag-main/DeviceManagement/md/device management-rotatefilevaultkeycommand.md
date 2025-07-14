

- Device Management
-  RotateFileVaultKeyCommand 

Device Management Command

# RotateFileVaultKeyCommand

The command to change the FileVault primary password.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object RotateFileVaultKeyCommand
```

## Properties

`Command`

RotateFileVaultKeyCommand.Command

 (Required) 

The command dictionary.

`CommandUUID`

`string`

 (Required) 

The unique identifier of the command.

## Topics

### Commands

object RotateFileVaultKeyCommand.Command

The request dictionary to change the FileVault primary password on a device.

## See Also

### Command and Response

object RotateFileVaultKeyResponse

A response from the device after it processes the command to change the FileVault primary password.

