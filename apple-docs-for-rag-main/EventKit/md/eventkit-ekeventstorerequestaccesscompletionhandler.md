

- EventKit
-  EKEventStoreRequestAccessCompletionHandler 

Type Alias

# EKEventStoreRequestAccessCompletionHandler

The signature for a closure that EventKit calls when requesting access to event and reminder data.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
typealias EKEventStoreRequestAccessCompletionHandler = (Bool, (any Error)?) -> Void
```

## Parameters 

`granted`  

true if the user allows the app to access data in the event store; otherwise, false.

`error`  

The error that occurred, if any; otherwise, `nil`.

## See Also

### Requesting access to events and reminders

func requestWriteOnlyAccessToEvents(completion: EKEventStoreRequestAccessCompletionHandler)

Prompts the person using your app to grant or deny write access to event data.

func requestFullAccessToEvents(completion: EKEventStoreRequestAccessCompletionHandler)

Prompts people to grant or deny read and write access to event data.

func requestFullAccessToReminders(completion: EKEventStoreRequestAccessCompletionHandler)

Prompts people to grant or deny read and write access to reminders.

class func authorizationStatus(for: EKEntityType) -> EKAuthorizationStatus

Determines the authorization status for the given entity type.

enum EKAuthorizationStatus

The current authorization status for a specific entity type.

NSCalendarsFullAccessUsageDescription

A message that tells people why the app is requesting access to read and write their calendar data.

NSCalendarsWriteOnlyAccessUsageDescription

A message that tells people why the app is requesting access to create calendar events.

NSRemindersFullAccessUsageDescription

A message that tells people why the app is requesting access to read and write their reminders data.

