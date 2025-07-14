

- Device Management
- NSExtensionMappingsResponse
-  NSExtensionMappingsResponse.ErrorChainItem 

Device Management Command

# NSExtensionMappingsResponse.ErrorChainItem

A dictionary that describes an error chain item.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object NSExtensionMappingsResponse.ErrorChainItem
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

object NSExtensionMappingsResponse.ExtensionsItem

A dictionary that contains information about an extension.

