

- EventKit
- EKEventStore
-  requestFullAccessToReminders(completion:) 

Instance Method

# requestFullAccessToReminders(completion:)

Prompts people to grant or deny read and write access to reminders.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
func requestFullAccessToReminders(completion: @escaping EKEventStoreRequestAccessCompletionHandler)
```

``` source
func requestFullAccessToReminders() async throws -> Bool
```

## Parameters 

`completion`  

The block to call when the request completes.

## Mentioned in 

Accessing the event store

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func requestFullAccessToReminders() async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Requesting access to an event store asynchronously prompts people for permission to use their data. The operating system only prompts them the first time your app requests access to reminders; any subsequent instantiations of EKEventStore uses existing permissions. When they grant or deny access, EventKit calls the completion handler on an arbitrary queue.

Your app isn’t blocked while the person decides to grant or deny permission. Because they may deny permission, your app should handle cases where it doesn’t receive access to the event store.

Important

If your app has never requested access, you must request access to reminders before attempting to fetch or create them. If you request reminders before prompting the person for access with this method, you’ll need to reset the event store with the reset() method to receive data after they grant access.

## See Also

### Requesting access to events and reminders

func requestWriteOnlyAccessToEvents(completion: EKEventStoreRequestAccessCompletionHandler)

Prompts the person using your app to grant or deny write access to event data.

func requestFullAccessToEvents(completion: EKEventStoreRequestAccessCompletionHandler)

Prompts people to grant or deny read and write access to event data.

class func authorizationStatus(for: EKEntityType) -> EKAuthorizationStatus

Determines the authorization status for the given entity type.

enum EKAuthorizationStatus

The current authorization status for a specific entity type.

typealias EKEventStoreRequestAccessCompletionHandler

The signature for a closure that EventKit calls when requesting access to event and reminder data.

NSCalendarsFullAccessUsageDescription

A message that tells people why the app is requesting access to read and write their calendar data.

NSCalendarsWriteOnlyAccessUsageDescription

A message that tells people why the app is requesting access to create calendar events.

NSRemindersFullAccessUsageDescription

A message that tells people why the app is requesting access to read and write their reminders data.

