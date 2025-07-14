

- Device Management
- ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
- ContentCachingInformationResponse.StatusResponse.PeersItem
-  ContentCachingInformationResponse.StatusResponse.PeersItem.Alert 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.PeersItem.Alert

A dictionary that describes a peer content cache alert.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.PeersItem.Alert
```

## Properties

`addresses`

`[string]`

An array of local IP addresses of peer content caches.

`className`

`string`

 (Required) 

The type of the alert.

Possible Values: `AssetCachePeerCycleAlert, AssetCacheUnfriendlyPeerAlert`

`peerAddress`

`string`

The local IP address of a peer content cache.

`postDate`

`date`

 (Required) 

The date of the alert.

## See Also

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.PeersItem.Details

A dictionary that contains additional details about the peer content cache.

