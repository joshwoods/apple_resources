

- Device Management
- RotateFileVaultKeyResponse
-  RotateFileVaultKeyResponse.RotateResult 

Device Management Command

# RotateFileVaultKeyResponse.RotateResult

The result of rotating the personal recovery key.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object RotateFileVaultKeyResponse.RotateResult
```

## Properties

`EncryptedNewRecoveryKey`

`data`

A new personal recovery key that is encrypted using a `ReplyEncryptionCertificate` as a CMS-compliant envelope.

## See Also

### Commands

object RotateFileVaultKeyResponse.ErrorChainItem

A dictionary that describes an error chain item.

