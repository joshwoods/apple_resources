

- Contacts
- CNAuthorizationStatus
-  CNAuthorizationStatus.limited 

Case

# CNAuthorizationStatus.limited

The app has access to a limited subset of contacts, chosen by the person using the app.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+watchOS 11.0+

``` source
case limited
```

## Mentioned in 

Accessing the contact store

## Discussion

A person can give your app limited access to their contacts by choosing this option when your app first attempts to authorize for accessing contacts. Thereafter, the person can maintain the set of contacts exposed to your app by managing them in the Settings app.

Your app can prompt the person to add contacts to the limited-access set by displaying a ContactAccessButton, in association with a search UI your app provides. You can also display a picker to add contacts with the SwiftUI view modifier contactAccessPicker(isPresented:completionHandler:).

## See Also

### Authorization statuses

case notDetermined

The user has not yet made a choice regarding whether the application may access contact data.

case restricted

The application is not authorized to access contact data. The user cannot change this application’s status, possibly due to active restrictions such as parental controls being in place.

case denied

The user explicitly denied access to contact data for the application.

case authorized

The application is authorized to access contact data.

