

- App Store Connect API
-  AppInfo 

Object

# AppInfo

The data structure that represent an App Infos resource.

App Store Connect API 1.2+

``` source
object AppInfo
```

## Properties

`attributes`

AppInfo.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

AppInfo.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appInfos`

## Topics

### Objects

object AppInfo.Attributes

Attributes that describe an App Infos resource.

object AppInfo.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object AppInfoResponse

A response that contains a single App Infos resource.

object AppInfosResponse

A response that contains a list of App Info resources.

object AppInfoUpdateRequest

The request body you use to update an App Info.

