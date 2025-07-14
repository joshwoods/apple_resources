

- App Store Connect API
-  AppStoreVersionReleaseRequest 

Object

# AppStoreVersionReleaseRequest

The data structure that represents an App Store Version Release Request resource.

App Store Connect API 1.5+

``` source
object AppStoreVersionReleaseRequest
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`links`

ResourceLinks

Navigational links that include the self-link.

`type`

`string`

 (Required) 

The resource type.

Value: `appStoreVersionReleaseRequests`

## See Also

### Objects

object AppStoreVersionReleaseRequestCreateRequest

The request body you use to manually release an App Store approved version of your app.

object AppStoreVersionReleaseRequestResponse

A response that contains a single App Store Version Release Request resource.

