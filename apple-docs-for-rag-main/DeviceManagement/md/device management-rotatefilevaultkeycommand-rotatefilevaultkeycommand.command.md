

- Device Management
- RotateFileVaultKeyCommand
-  RotateFileVaultKeyCommand.Command 

Device Management Command

# RotateFileVaultKeyCommand.Command

The request dictionary to change the FileVault primary password on a device.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object RotateFileVaultKeyCommand.Command
```

## Properties

`FileVaultUnlock`

RotateFileVaultKeyCommand.Command.FileVaultUnlock

 (Required) 

A dictionary that contains FileVault unlock options.

`KeyType`

`string`

 (Required) 

The type of FileVault key you want to change the password for. Set this value to `personal` and set a value for `Password` in the `FileVaultUnlock` dictionary to enable unlocking a device with a password. Set this value to `institutional` and set values for `PrivateKeyExport` and `PrivateKeyExportPassword` in the `FileVaultUnlock` dictionary.

Possible Values: `personal, institutional`

`NewCertificate`

`data`

A DER-encoded certificate for creating a new institutional recovery key, which the system requires if `KeyType` is `institutional`.

`ReplyEncryptionCertificate`

`data`

A DER-encoded certificate for encrypting the new personal recovery key in a wrapper conforming to the IETF Cryptographic Message Syntax (CMS) standard.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to change the FileVault primary password on a device.

Value: `RotateFileVaultKey`

## Topics

### Commands

object RotateFileVaultKeyCommand.Command.FileVaultUnlock

A dictionary that contains FileVault unlock options.

