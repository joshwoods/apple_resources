

- Device Management
- ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
-  ContentCachingInformationResponse.StatusResponse.CacheDetails 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.CacheDetails

A dictionary that describes disk space the content cache uses.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.CacheDetails
```

## Properties

`Category Name`

`integer`

 (Required) 

The amount of disk space, in bytes, that this category of cached content uses.

## See Also

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.AlertsItem

A dictionary that describes an alert from the content cache.

object ContentCachingInformationResponse.StatusResponse.DataMigrationError

A dictionary that describes a data migration error.

object ContentCachingInformationResponse.StatusResponse.ParentsItem

A dictionary that describes a parent content cache.

object ContentCachingInformationResponse.StatusResponse.PeersItem

A dictionary that describes a peer content cache.

object ContentCachingInformationResponse.StatusResponse.AlertsForPeerFilterRanges

A dictionary that contains alerts for peer filter ranges.

