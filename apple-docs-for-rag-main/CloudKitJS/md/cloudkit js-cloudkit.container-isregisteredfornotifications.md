

- CloudKit JS
- CloudKit.Container
-  isRegisteredForNotifications 

Instance Property

# isRegisteredForNotifications

Boolean value indicating whether this container is registered to receive push notifications.

CloudKit JS 1.0+

``` source
attribute Boolean isRegisteredForNotifications;
```

## Discussion

`true` if the container is registered to receive push notifications; otherwise, `false`.

## See Also

### Receiving Notifications

addNotificationListener

Adds a function to call when a push notification occurs.

removeNotificationListener

Removes a function to call when a push notification occurs.

registerForNotifications

Registers to receive push notifications.

unregisterForNotifications

Unregisters to receive push notifications.

