

- Device Management
- RotateFileVaultKeyResponse
-  RotateFileVaultKeyResponse.ErrorChainItem 

Device Management Command

# RotateFileVaultKeyResponse.ErrorChainItem

A dictionary that describes an error chain item.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object RotateFileVaultKeyResponse.ErrorChainItem
```

## Properties

`ErrorCode`

`integer`

 (Required) 

The error code.

`ErrorDomain`

`string`

 (Required) 

The error domain.

`LocalizedDescription`

`string`

 (Required) 

A description of the error in the device’s localized language.

`USEnglishDescription`

`string`

A description of the error in U.S. English.

## See Also

### Commands

object RotateFileVaultKeyResponse.RotateResult

The result of rotating the personal recovery key.

