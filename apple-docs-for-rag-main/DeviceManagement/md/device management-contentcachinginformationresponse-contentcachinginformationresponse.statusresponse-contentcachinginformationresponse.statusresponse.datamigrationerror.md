

- Device Management
- ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
-  ContentCachingInformationResponse.StatusResponse.DataMigrationError 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.DataMigrationError

A dictionary that describes a data migration error.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.DataMigrationError
```

## Properties

`code`

`integer`

 (Required) 

The error code.

`domain`

`string`

 (Required) 

The error domain.

`userInfo`

ContentCachingInformationResponse.StatusResponse.DataMigrationError.UserInfo

A dictionary that contains additional information about the error.

## Topics

### User Information

object ContentCachingInformationResponse.StatusResponse.DataMigrationError.UserInfo

A dictionary that contains additional information about a data migration error.

## See Also

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.AlertsItem

A dictionary that describes an alert from the content cache.

object ContentCachingInformationResponse.StatusResponse.CacheDetails

A dictionary that describes disk space the content cache uses.

object ContentCachingInformationResponse.StatusResponse.ParentsItem

A dictionary that describes a parent content cache.

object ContentCachingInformationResponse.StatusResponse.PeersItem

A dictionary that describes a peer content cache.

object ContentCachingInformationResponse.StatusResponse.AlertsForPeerFilterRanges

A dictionary that contains alerts for peer filter ranges.

