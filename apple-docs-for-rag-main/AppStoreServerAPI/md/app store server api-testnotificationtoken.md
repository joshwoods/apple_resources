

- App Store Server API
-  testNotificationToken 

Type

# testNotificationToken

A unique identifier for a notification test that the App Store server sends to your server.

App Store Server API 1.5+

``` source
string testNotificationToken
```

## Discussion

You receive a `testNotificationToken` when you call the Request a Test Notification endpoint. Use the `testNotificationToken` to learn your server’s response to the test by calling Get Test Notification Status.

