

- App Store Server Notifications
-  App Store Server Notifications V1 Deprecated

Web Service Endpoint

# App Store Server Notifications V1

Specify your secure server’s URL in App Store Connect to receive version 1 notifications.

App Store Server Notifications 1.0–2.8Deprecated

Deprecated

The App Store Server Notifications V1 endpoint and version 1 notifications are deprecated. Implement the App Store Server Notifications V2 endpoint on your server to receive version 2 notifications instead.

## URL

``` source
POST https://example.com/v1
```

## Response Codes

` 200 ``OK`

responseBodyV1

`OK`

The response body for a version 1 notification.

Content-Type: application/json

## Mentioned in 

App Store Server Notifications changelog

Receiving App Store Server Notifications

## Discussion

To receive server notifications from the App Store, provide your secure server’s HTTPS URL in App Store Connect. For more information, see Enabling App Store Server Notifications. To secure your server and receive notifications, your server must support the Transport Layer Security (TLS) protocol version 1.2 or later.

Upon receiving a server notification, respond to the App Store with an HTTP status code of `200` if the post was successful. If the post was unsuccessful, send HTTP `50x` or `40x` to have the App Store retry the notification. For more information, see Responding to App Store Server Notifications.

Note

For version 2 notifications, see App Store Server Notifications V2.

## See Also

### Version 1 notifications

object responseBodyV1

The response body containing JSON data that the App Store sends in a version 1 server notification.

Deprecated

type notification_type

The type that describes the in-app purchase event for which the App Store sends the version 1 notification.

Deprecated

