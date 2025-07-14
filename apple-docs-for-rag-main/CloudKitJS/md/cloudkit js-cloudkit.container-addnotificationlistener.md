

- CloudKit JS
- CloudKit.Container
-  addNotificationListener 

Instance Method

# addNotificationListener

Adds a function to call when a push notification occurs.

CloudKit JS 1.0+

``` source
void addNotificationListener(
 function listener
);
```

## Parameters 

`listener`  

The function to call when a push notification occurs. The function must have a single argument that is a CloudKit.Notification object.

## Discussion

To subscribe to changes and register for push notifications, see `saveSubscription` in the CloudKit.Database class.

## See Also

### Receiving Notifications

removeNotificationListener

Removes a function to call when a push notification occurs.

registerForNotifications

Registers to receive push notifications.

unregisterForNotifications

Unregisters to receive push notifications.

isRegisteredForNotifications

Boolean value indicating whether this container is registered to receive push notifications.

