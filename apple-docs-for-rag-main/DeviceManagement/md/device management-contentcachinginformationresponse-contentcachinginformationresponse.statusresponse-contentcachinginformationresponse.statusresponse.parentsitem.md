

- Device Management
- ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
-  ContentCachingInformationResponse.StatusResponse.ParentsItem 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.ParentsItem

A dictionary that describes a parent content cache.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.ParentsItem
```

## Properties

`address`

`string`

 (Required) 

The local IP address of the parent content cache.

`alert`

ContentCachingInformationResponse.StatusResponse.ParentsItem.Alert

A dictionary that describes an alert related to the parent content cache.

`details`

ContentCachingInformationResponse.StatusResponse.ParentsItem.Details

 (Required) 

A dictionary that contains additional details about the parent content cache.

`guid`

`string`

 (Required) 

The unique identifier of the parent content cache.

`healthy`

`boolean`

 (Required) 

If `true,` the parent content cache is able to respond to requests from this content cache.

`port`

`integer`

 (Required) 

The IP port number the parent content cache listens to for requests.

`version`

`string`

 (Required) 

The version number of the parent content cache software.

## Topics

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.ParentsItem.Alert

A dictionary that describes a parent content cache alert.

object ContentCachingInformationResponse.StatusResponse.ParentsItem.Details

A dictionary that contains additional details about the parent content cache.

## See Also

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.AlertsItem

A dictionary that describes an alert from the content cache.

object ContentCachingInformationResponse.StatusResponse.CacheDetails

A dictionary that describes disk space the content cache uses.

object ContentCachingInformationResponse.StatusResponse.DataMigrationError

A dictionary that describes a data migration error.

object ContentCachingInformationResponse.StatusResponse.PeersItem

A dictionary that describes a peer content cache.

object ContentCachingInformationResponse.StatusResponse.AlertsForPeerFilterRanges

A dictionary that contains alerts for peer filter ranges.

