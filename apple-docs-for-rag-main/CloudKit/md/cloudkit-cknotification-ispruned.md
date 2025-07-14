

- CloudKit
- CKNotification
-  isPruned 

Instance Property

# isPruned

A Boolean value that indicates whether the system removes some push notification content before delivery.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var isPruned: Bool { get }
```

## Discussion

The server may truncate the payload data of a push notification if the size of that data exceeds the allowed maximum. For notifications you create using a payload dictionary, the value of this property is true if the payload data doesn’t contain all information regarding the change. The value is false if the payload data is complete.

For notifications you fetch from the database using a `CKFetchNotificationChangesOperation` operation, this property’s value is always true.

When CloudKit must remove payload data, it removes it in a specific order. This class’s properties are among the last that CloudKit removes because they define information about how to deliver the push notification. The following list shows the properties that CloudKit removes, and the order for removing them:

1.  containerIdentifier

2.  Keys that subclasses of `CKNotification` define.

3.  soundName

4.  alertLaunchImage

5.  alertActionLocalizationKey

6.  alertBody

7.  alertLocalizationArgs

8.  alertLocalizationKey

9.  badge

10. notificationID

