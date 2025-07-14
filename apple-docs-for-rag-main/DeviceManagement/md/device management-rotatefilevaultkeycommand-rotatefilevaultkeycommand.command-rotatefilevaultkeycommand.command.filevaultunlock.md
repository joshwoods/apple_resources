

- Device Management
- RotateFileVaultKeyCommand
- RotateFileVaultKeyCommand.Command
-  RotateFileVaultKeyCommand.Command.FileVaultUnlock 

Device Management Command

# RotateFileVaultKeyCommand.Command.FileVaultUnlock

A dictionary that contains FileVault unlock options.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object RotateFileVaultKeyCommand.Command.FileVaultUnlock
```

## Properties

`Password`

`string`

A FileVault user’s password, or if using a CoreStorage volume, the personal recovery key.

`PrivateKeyExport`

`data`

Deprecated 

The data for a .p12 export of the private key for the current institutional recovery key, which requires that `KeyType` is `institutional`. The system ignores this key on APFS volumes.

`PrivateKeyExportPassword`

`string`

Deprecated 

The password for `PrivateKeyExport`. Either `Password` or both `PrivateKeyExport` and `PrivateKeyExportPassword` must be present. The system ignores this key on APFS volumes.

