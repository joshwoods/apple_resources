

- EventKit
- EKEventStore
-  requestWriteOnlyAccessToEvents(completion:) 

Instance Method

# requestWriteOnlyAccessToEvents(completion:)

Prompts the person using your app to grant or deny write access to event data.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
func requestWriteOnlyAccessToEvents(completion: @escaping EKEventStoreRequestAccessCompletionHandler)
```

``` source
func requestWriteOnlyAccessToEvents() async throws -> Bool
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
func requestWriteOnlyAccessToEvents() async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Requesting access to an event store asynchronously prompts people for permission to use their data. The operating system only prompts them the first time your app requests write-only event access; any subsequent instantiations of EKEventStore uses existing permissions. When they grant or deny access, EventKit calls the completion handler on an arbitrary queue.

Important

If your app has never requested access, you must request write-only or full access to events before attempting to create them. If you request events before prompting the user for access with this method, you’ll need to reset the event store with the reset() method to receive data after the user grants access.

Your app isn’t blocked while the person decides to grant or deny permission. Because they may deny permission, your app needs to handle the case where it doesn’t receive access to the event store.

If the person grants permission, your app receives write-only access to the event store. Your app can create events, but it can’t access any of the existing calendars and events on the device, including events your app created. API calls to read event data from the event store don’t return any events.

Note

Your iOS or Mac Catalyst app can present an EKEventEditViewController to let your user create events without requesting access to the event store. If your app creates events without using EKEventEditViewController, you must request at least write-only access to event data.

## See Also

### Requesting access to events and reminders

func requestFullAccessToEvents(completion: EKEventStoreRequestAccessCompletionHandler)

Prompts people to grant or deny read and write access to event data.

func requestFullAccessToReminders(completion: EKEventStoreRequestAccessCompletionHandler)

Prompts people to grant or deny read and write access to reminders.

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

