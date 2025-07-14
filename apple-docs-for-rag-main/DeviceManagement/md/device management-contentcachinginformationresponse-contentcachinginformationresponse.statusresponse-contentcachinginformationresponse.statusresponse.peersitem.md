

- Device Management
- ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
-  ContentCachingInformationResponse.StatusResponse.PeersItem 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.PeersItem

A dictionary that describes a peer content cache.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.PeersItem
```

## Properties

`address`

`string`

 (Required) 

The local IP address of the peer content cache.

`alert`

ContentCachingInformationResponse.StatusResponse.PeersItem.Alert

A dictionary that describes an alert related to the peer content cache.

`details`

ContentCachingInformationResponse.StatusResponse.PeersItem.Details

 (Required) 

A dictionary that contains additional details about the peer content cache.

`friendly`

`boolean`

 (Required) 

If `true`, the peer content cache is able to respond to requests from the content cache.

`guid`

`string`

 (Required) 

The unique identifier of the peer content cache.

`healthy`

`boolean`

 (Required) 

If `true`, the peer content cache is able to respond to requests from the content cache.

`port`

`integer`

 (Required) 

The IP port number the peer content cache listens to for requests.

`version`

`string`

 (Required) 

The version number of the peer content cache software.

## Topics

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.PeersItem.Alert

A dictionary that describes a peer content cache alert.

object ContentCachingInformationResponse.StatusResponse.PeersItem.Details

A dictionary that contains additional details about the peer content cache.

## See Also

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.AlertsItem

A dictionary that describes an alert from the content cache.

object ContentCachingInformationResponse.StatusResponse.CacheDetails

A dictionary that describes disk space the content cache uses.

object ContentCachingInformationResponse.StatusResponse.DataMigrationError

A dictionary that describes a data migration error.

object ContentCachingInformationResponse.StatusResponse.ParentsItem

A dictionary that describes a parent content cache.

object ContentCachingInformationResponse.StatusResponse.AlertsForPeerFilterRanges

A dictionary that contains alerts for peer filter ranges.

