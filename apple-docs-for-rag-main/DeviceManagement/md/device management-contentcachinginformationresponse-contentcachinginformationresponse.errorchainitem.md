

- Device Management
- ContentCachingInformationResponse
-  ContentCachingInformationResponse.ErrorChainItem 

Device Management Command

# ContentCachingInformationResponse.ErrorChainItem

A dictionary that describes an error chain item.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.ErrorChainItem
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

object ContentCachingInformationResponse.StatusResponse

A dictionary that contains the status of content caching on a device.

