

- Device Management
- ContentCachingInformationResponse
- 
  - ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
- ContentCachingInformationResponse.StatusResponse.ParentsItem
- ContentCachingInformationResponse.StatusResponse.ParentsItem.Details
-  ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Local-network 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Local-network

A dictionary that describes the parent content cache’s connection to its local network.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Local-network
```

## Properties

`speed`

`integer`

The transfer speed, in megabits per second, of the parent content cache’s connection to its local network.

`wired`

`boolean`

If `true`, the parent content cache has a wired connection to its local network. If `false`, it has a wireless connection; for example, Wi-Fi.

Default: `false`

## See Also

### Commands

object ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Capabilities

A dictionary that describes the capabilities of the parent content cache.

