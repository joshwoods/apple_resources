

- EventKit
- EKEventStore
-  requestAccess(to:completion:) Deprecated

Instance Method

# requestAccess(to:completion:)

Prompts the person using your app to grant or deny access to event or reminder data.

iOS 6.0–17.0DeprecatediPadOS 6.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–10.0Deprecated

``` source
func requestAccess(
    to entityType: EKEntityType,
    completion: @escaping EKEventStoreRequestAccessCompletionHandler
)
```

``` source
func requestAccess(to entityType: EKEntityType) async throws -> Bool
```

Deprecated

On iOS 17 and later, this method doesn’t prompt for access and immediately calls the completion block with an error.

If your app only uses EKEventEditViewController to let your user create and save calendar events, don’t request events access. Use requestWriteOnlyAccessToEvents(completion:) to create calendar events. Use requestFullAccessToEvents(completion:) to read and write calendar events. Use requestFullAccessToReminders(completion:) to read and write reminders.

## Parameters 

`entityType`  

The event or reminder entity type.

`completion`  

The block to call when the request completes.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func requestAccess(to entityType: EKEntityType) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

In iOS 6 and later, requesting access to an event store asynchronously prompts your users for permission to use their data. The user is only prompted the first time your app requests access to an entity type; any subsequent instantiations of `EKEventStore` uses existing permissions. When the user taps to grant or deny access, the completion handler will be called on an arbitrary queue. Your app isn’t blocked while the user decides to grant or deny permission.

After users choose their permission level, the event store either calls the completion handler or broadcasts an EKEventStoreChangedNotification. The completion handler is called on iOS 6 and later, and the notification is broadcasted on iOS 5. Because users may deny access to the event store, your app should handle an empty data case.

Important

If your app has never requested access before, you must request access to events or reminders before attempting to fetch or create them. If you request data before prompting the user for access with this method, you’ll need to reset the event store with the reset() method in order to start receiving data after the user grants access.

