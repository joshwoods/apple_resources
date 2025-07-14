

- Device Management
- ContentCachingInformationResponse
- 
  - ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
- ContentCachingInformationResponse.StatusResponse.PeersItem
- ContentCachingInformationResponse.StatusResponse.PeersItem.Details
-  ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Local-network 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Local-network

The network details about the peer cache.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Local-network
```

## Properties

`speed`

`integer`

The transfer speed, in megabits per second, of the peer content cache’s connection to its local network.

`wired`

`boolean`

If `true`, the peer content cache has a wired connection to its local network. If `false`, it has a wireless connection; for example, Wi-Fi.

Default: `false`

## See Also

### Commands

object ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Capabilities

The capabilities of the peer content cache.

