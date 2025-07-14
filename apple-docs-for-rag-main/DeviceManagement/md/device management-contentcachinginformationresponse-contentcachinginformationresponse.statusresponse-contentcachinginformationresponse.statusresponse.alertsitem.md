

- Device Management
- ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
-  ContentCachingInformationResponse.StatusResponse.AlertsItem 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.AlertsItem

A dictionary that describes an alert from the content cache.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.AlertsItem
```

## Properties

`cacheLimit`

`integer`

The limit, in bytes, for the content cache at the time of the alert. This value only applies to `AssetCacheLowSpaceAlert` and `AssetCacheNoSpaceAlert` types.

`className`

`string`

 (Required) 

The type of the alert.

Possible Values: `AssetCacheLowSpaceAlert, AssetCacheNoSpaceAlert, AssetCacheRegistrationRejectedAlert, AssetCacheRegistrationUnavailableAlert, AssetCacheResourceMissingAlert`

`pathPreventingAccess`

`string`

The subpath of the resource that was missing or inaccessible at the time of the alert. This value only applies to the `AssetCacheResourceMissingAlert` type.

`postDate`

`date`

 (Required) 

The date of the alert.

`reservedVolumeSpace`

`integer`

The space, in bytes, that the system reserves at the time of the alert. This value only applies to the `AssetCacheLowSpaceAlert` and `AssetCacheNoSpaceAlert` types.

`resource`

`string`

The resource that was missing or inaccessible at the time of the alert. This value only applies to the `AssetCacheResourceMissingAlert` type.

## See Also

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.CacheDetails

A dictionary that describes disk space the content cache uses.

object ContentCachingInformationResponse.StatusResponse.DataMigrationError

A dictionary that describes a data migration error.

object ContentCachingInformationResponse.StatusResponse.ParentsItem

A dictionary that describes a parent content cache.

object ContentCachingInformationResponse.StatusResponse.PeersItem

A dictionary that describes a peer content cache.

object ContentCachingInformationResponse.StatusResponse.AlertsForPeerFilterRanges

A dictionary that contains alerts for peer filter ranges.

