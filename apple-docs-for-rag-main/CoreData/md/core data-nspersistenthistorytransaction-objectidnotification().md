

- Core Data
- NSPersistentHistoryTransaction
-  objectIDNotification() 

Instance Method

# objectIDNotification()

Obtains a notification for use in merging the transaction’s changes into a managed object context.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func objectIDNotification() -> Notification
```

## Return Value

An `NSManagedObjectContextDidSaveObjectIDsNotification` notification.

## Mentioned in 

Consuming relevant store changes

## Discussion

To merge the relevant changes into your view context, first obtain a notification by calling `objectIDNotification()` on the transaction. Then, pass the notification to mergeChanges(fromContextDidSave:).

