

- CoreLocationUI
-  LocationButton 

Structure

# LocationButton

A SwiftUI button that grants one-time location authorization.

CoreLocationUISwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
struct LocationButton
```

## Overview

`LocationButton` simplifies requesting one-time authorization to access location data. Add this button to your SwiftUI user interface in situations when users may want to grant temporary access to their location data each time they use a particular feature of your app.

The first time a user taps this button, Core Location asks the user to confirm that they’re comfortable using this UI element when they want to grant temporary access to their location data. If the user agrees, the app receives temporary CLAuthorizationStatus.authorizedWhenInUse authorization, like when the user chooses *Allow Once* in response to your app’s standard location authorization request. This temporary authorization expires when your app is no longer in use.

After the user agrees to using `LocationButton`, the button becomes approved to request future authorizations without displaying an additional alert to the user. The next time the user taps it, this button simply grants one-time authorization without requiring confirmation.

After you receive this temporary authorization, fetch the user’s location using the Core Location API and perform any app-specific tasks related to that location data. Connect the button to initiate the tasks you want to perform after getting authorization by specifying an action when you create the button. Keep in mind that this action activates every time the user taps this button, regardless of whether the app already has location authorization.

Create a `LocationButton` in SwiftUI like this:

```
LocationButton(.currentLocation) {
    // Fetch location with Core Location.
}
.symbolVariant(.fill)
.labelStyle(.titleAndIcon)
```

Important

When a user taps the button, it only provides one-time authorization to fetch location data — not the location data itself. For more details about fetching location data, see Configuring your app to use location services.

Configure the button to display an icon, a label, or both using the labelStyle(_:) view modifier. If you include an icon, you can customize its appearance using the symbolVariant(_:) modifier. For design guidance, see Human Interface Guidelines.

## Topics

### Creating a location button

init(LocationButton.Title?, action: () -> Void)

Creates a location button with the specified title and action.

struct Title

Constants that specify the text of a button title.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Location authorization

Sharing Your Location to Find a Park

Ask for location access using a customizable location button.

class CLLocationButton

A button that grants one-time location authorization.

