

- Device Management
- ProfileListResponse
- ProfileListResponse.ProfileListItem
-  ProfileListResponse.ProfileListItem.PayloadContentItem 

Device Management Command

# ProfileListResponse.ProfileListItem.PayloadContentItem

A dictionary that describes a profile payload content item.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ProfileListResponse.ProfileListItem.PayloadContentItem
```

## Properties

`PayloadDescription`

`string`

A description of the payload.

`PayloadDisplayName`

`string`

The human-readable name of the payload.

`PayloadIdentifier`

`string`

 (Required) 

The reverse-DNS-style identifier of the payload, such as `com.example.mypayload`.

`PayloadOrganization`

`string`

The human-readable name of the organization that provided the payload.

`PayloadType`

`string`

 (Required) 

The type of payload, such as `com.apple.wifi.managed`.

`PayloadUUID`

`string`

 (Required) 

The unique identifier of the payload.

`PayloadVersion`

`integer`

 (Required) 

The version of the payload.

## See Also

### Commands

object ProfileListResponse.ProfileListItem

A dictionary that describes a profile list item.

object ProfileListResponse.ErrorChainItem

A dictionary that describes an error chain item.

