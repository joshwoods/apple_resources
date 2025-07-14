

- Device Management
- ContentCachingInformationResponse
- ContentCachingInformationResponse.StatusResponse
- ContentCachingInformationResponse.StatusResponse.ParentsItem
-  ContentCachingInformationResponse.StatusResponse.ParentsItem.Details 

Device Management Command

# ContentCachingInformationResponse.StatusResponse.ParentsItem.Details

A dictionary that contains additional details about the parent content cache.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationResponse.StatusResponse.ParentsItem.Details
```

## Properties

`ac-power`

`boolean`

If `true`, the parent content cache power source is AC; otherwise, an internal battery provides its power.

Default: `false`

`cache-size`

`integer`

The maximum amount of disk space, in bytes, available to the parent content cache.

`capabilities`

ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Capabilities

A dictionary that describes the capabilities of the parent content cache.

`is-portable`

`boolean`

If `true`, the parent content cache computer is portable; for example, a laptop.

Default: `false`

`local-network`

ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Local-network

A dictionary that describes the parent content cache’s connection to its local network.

## Topics

### Commands

object ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Capabilities

A dictionary that describes the capabilities of the parent content cache.

object ContentCachingInformationResponse.StatusResponse.ParentsItem.Details.Local-network

A dictionary that describes the parent content cache’s connection to its local network.

## See Also

### Response Dictionaries

object ContentCachingInformationResponse.StatusResponse.ParentsItem.Alert

A dictionary that describes a parent content cache alert.

