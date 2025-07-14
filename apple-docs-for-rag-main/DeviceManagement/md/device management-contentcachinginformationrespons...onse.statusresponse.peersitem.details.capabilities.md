

- Device Management
- ContentCachingInformationResponse
- 
  - ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
- ContentCachingInformationResponse.StatusResponse.PeersItem
- ContentCachingInformationResponse.StatusResponse.PeersItem.Details
-  ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Capabilities 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Capabilities

The capabilities of the peer content cache.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Capabilities
```

## Properties

`im`

`boolean`

If `true`, the peer content cache is capable of imports and uploads.

Default: `false`

`ns`

`boolean`

If `true`, the peer content cache is capable of handling namespaces, which is an aspect of personal caching.

Default: `false`

`pc`

`boolean`

If `true`, the peer content cache is capable of caching personal iCloud content.

Default: `false`

`query-parameters`

`boolean`

If `true`, the peer content cache is capable of handling query parameters in URLs.

Default: `false`

`sc`

`boolean`

If `true`, the peer content cache is capable of caching shared non-iCloud content.

Default: `false`

`ur`

`boolean`

If `true`, the peer content cache is capable of prioritizing imports and uploads.

Default: `false`

## See Also

### Commands

object ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Local-network

The network details about the peer cache.

