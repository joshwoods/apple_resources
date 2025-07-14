

- App Store Connect API
-  BuildBetaNotification 

Object

# BuildBetaNotification

The data structure that represents a Build Beta Notifications resource.

App Store Connect API 1.0+

``` source
object BuildBetaNotification
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

Value: `buildBetaNotifications`

## See Also

### Objects

object BuildBetaNotificationCreateRequest

The request body you use to create a Build Beta Notification.

object BuildBetaNotificationResponse

A response that contains a single Build Beta Notifications resource.

