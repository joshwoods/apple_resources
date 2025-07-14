

- Contacts
-  CNAuthorizationStatus 

Enumeration

# CNAuthorizationStatus

An authorization status the user can grant for an app to access the specified entity type.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
enum CNAuthorizationStatus
```

## Topics

### Authorization statuses

case notDetermined

The user has not yet made a choice regarding whether the application may access contact data.

case restricted

The application is not authorized to access contact data. The user cannot change this application’s status, possibly due to active restrictions such as parental controls being in place.

case denied

The user explicitly denied access to contact data for the application.

case authorized

The application is authorized to access contact data.

case limited

The app has access to a limited subset of contacts, chosen by the person using the app.

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

### Requesting access to the user’s contacts

func requestAccess(for: CNEntityType, completionHandler: (Bool, (any Error)?) -> Void)

Requests access to the user’s contacts.

class func authorizationStatus(for: CNEntityType) -> CNAuthorizationStatus

Returns the current authorization status to access the contact data.

enum CNEntityType

The entities the user can grant access to.

