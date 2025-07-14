

- Device Management
- ContentCachingInformationResponse
- 
  - ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
- ContentCachingInformationResponse.StatusResponse.ParentsItem
- ContentCachingInformationResponse.StatusResponse.ParentsItem.Details
-  ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Capabilities 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Capabilities

A dictionary that describes the capabilities of the parent content cache.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Capabilities
```

## Properties

`im`

`boolean`

If `true`, the parent content cache is capable of imports and uploads.

Default: `false`

`ns`

`boolean`

If `true`, the parent content cache is capable of handling namespaces, which is an aspect of personal caching.

Default: `false`

`pc`

`boolean`

If `true`, the parent content cache is capable of caching personal iCloud content.

Default: `false`

`query-parameters`

`boolean`

If `true`, the parent content cache is capable of handling query parameters in URLs.

Default: `false`

`sc`

`boolean`

If `true`, the parent content cache is capable of caching shared non-iCloud content.

Default: `false`

`ur`

`boolean`

If `true`, the parent content cache is capable of prioritizing imports and uploads.

Default: `false`

## See Also

### Commands

object ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Local-network

A dictionary that describes the parent content cache’s connection to its local network.

