

- Device Management
- ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
- ContentCachingInformationResponse.StatusResponse.ParentsItem
-  ContentCachingInformationResponse.StatusResponse.ParentsItem.Alert 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.ParentsItem.Alert

A dictionary that describes a parent content cache alert.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.ParentsItem.Alert
```

## Properties

`addresses`

`[string]`

 (Required) 

An array of local IP addresses of parent content caches.

`className`

`string`

 (Required) 

The type of the alert.

Possible Values: `AssetCacheParentCycleAlert, AssetCacheParentDepthAlert`

`postDate`

`date`

 (Required) 

The date of the alert.

## See Also

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.ParentsItem.Details

A dictionary that contains additional details about the parent content cache.

