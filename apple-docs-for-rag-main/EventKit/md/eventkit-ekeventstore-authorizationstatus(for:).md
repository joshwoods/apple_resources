

- EventKit
- EKEventStore
-  authorizationStatus(for:) 

Type Method

# authorizationStatus(for:)

Determines the authorization status for the given entity type.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+watchOS 2.0+

``` source
class func authorizationStatus(for entityType: EKEntityType) -> EKAuthorizationStatus
```

## Parameters 

`entityType`  

The event or reminder entity type.

## Return Value

The app’s authorization status of the given type.

## See Also

### Requesting access to events and reminders

func requestWriteOnlyAccessToEvents(completion: EKEventStoreRequestAccessCompletionHandler)

Prompts the person using your app to grant or deny write access to event data.

func requestFullAccessToEvents(completion: EKEventStoreRequestAccessCompletionHandler)

Prompts people to grant or deny read and write access to event data.

func requestFullAccessToReminders(completion: EKEventStoreRequestAccessCompletionHandler)

Prompts people to grant or deny read and write access to reminders.

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

