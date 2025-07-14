

- EventKit
-  EKAuthorizationStatus 

Enumeration

# EKAuthorizationStatus

The current authorization status for a specific entity type.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+watchOS 2.0+

``` source
enum EKAuthorizationStatus
```

## Topics

### Status

case fullAccess

The app has both read and write access to the requested entity type.

case writeOnly

The app has write-only access to the requested entity type.

case denied

The person explicitly denied access to the service for the app.

case notDetermined

The person hasn’t chosen whether the app may access the service.

case restricted

The app isn’t authorized to access the service.

### Deprecated values

static var authorized: EKAuthorizationStatus

The app can access the service.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

typealias EKEventStoreRequestAccessCompletionHandler

The signature for a closure that EventKit calls when requesting access to event and reminder data.

NSCalendarsFullAccessUsageDescription

A message that tells people why the app is requesting access to read and write their calendar data.

NSCalendarsWriteOnlyAccessUsageDescription

A message that tells people why the app is requesting access to create calendar events.

NSRemindersFullAccessUsageDescription

A message that tells people why the app is requesting access to read and write their reminders data.

