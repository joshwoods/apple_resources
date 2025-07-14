

- Contacts
- CNAuthorizationStatus
-  CNAuthorizationStatus.notDetermined 

Case

# CNAuthorizationStatus.notDetermined

The user has not yet made a choice regarding whether the application may access contact data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
case notDetermined
```

## Mentioned in 

Accessing the contact store

## See Also

### Authorization statuses

case restricted

The application is not authorized to access contact data. The user cannot change this application’s status, possibly due to active restrictions such as parental controls being in place.

case denied

The user explicitly denied access to contact data for the application.

case authorized

The application is authorized to access contact data.

case limited

The app has access to a limited subset of contacts, chosen by the person using the app.

