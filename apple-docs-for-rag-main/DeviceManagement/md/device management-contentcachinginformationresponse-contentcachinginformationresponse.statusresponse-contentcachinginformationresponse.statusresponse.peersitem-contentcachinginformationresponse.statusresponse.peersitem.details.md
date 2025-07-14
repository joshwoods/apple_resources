

- Device Management
- ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
- ContentCachingInformationResponse.StatusResponse.PeersItem
-  ContentCachingInformationResponse.StatusResponse.PeersItem.Details 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.PeersItem.Details

A dictionary that contains additional details about the peer content cache.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.PeersItem.Details
```

## Properties

`ac-power`

`boolean`

If `true`, the peer content cache power source is AC; otherwise, an internal battery provides its power.

Default: `false`

`cache-size`

`integer`

The maximum amount of disk space, in bytes, available to the peer content cache.

`capabilities`

ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Capabilities

A dictionary that describes the capabilities of the peer content cache.

`is-portable`

`boolean`

If `true`, the peer content cache computer is portable; for example, a laptop.

Default: `false`

`local-network`

ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Local-network

A dictionary that describes the peer content cache’s connection to its local network.

## Topics

### Commands

object ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Capabilities

The capabilities of the peer content cache.

object ContentCachingInformationResponse.StatusResponse.PeersItem.Details.Local-network

The network details about the peer cache.

## See Also

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.PeersItem.Alert

A dictionary that describes a peer content cache alert.

