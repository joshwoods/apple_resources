

- App Store Connect API
-  DevicesResponse 

Object

# DevicesResponse

A response that contains a list of Devices resources.

App Store Connect API 1.1+

``` source
object DevicesResponse
```

## Properties

`data`

`[`Device`]`

 (Required) 

The resource data.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

## See Also

### Related Documentation

List Devices

Find and list devices registered to your team.

### Objects

object Device

The data structure that represents a Devices resource.

object DevicesWithoutIncludesResponse

object DeviceCreateRequest

The request body you use to create a Device.

object DeviceUpdateRequest

The request body you use to update a Device.

object DeviceResponse

A response that contains a single Devices resource.

