

- CoreLocationUI
-  CLLocationButton 

Class

# CLLocationButton

A button that grants one-time location authorization.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor
class CLLocationButton
```

## Overview

`CLLocationButton` simplifies requesting one-time authorization to access location data. Add this button to your user interface in situations when users may want to grant temporary access to their location data each time they use a particular feature of your app.

The first time a user taps this button, Core Location asks the user to confirm that they’re comfortable using this UI element when they want to grant temporary access to their location data. If the user agrees, the app receives temporary CLAuthorizationStatus.authorizedWhenInUse authorization, like when the user chooses *Allow Once* in response to your app’s standard location authorization request. This temporary authorization expires when your app is no longer in use.

After the user agrees to using `CLLocationButton`, the button becomes approved to request future authorizations without displaying an additional alert to the user. The next time the user taps it, this button simply grants one-time authorization without requiring confirmation.

After you receive this temporary authorization, fetch the user’s location using the Core Location API and perform any app-specific tasks related to that location data. Connect the button to initiate the tasks you want to perform after getting authorization by adding a target and action to the button. Keep in mind that this action activates every time the user taps this button, regardless of whether the app already has location authorization.

Create a `CLLocationButton` in Interface Builder or in code, like this:

```
```

Important

When a user taps the button, it only provides one-time authorization to fetch location data — not the location data itself. For more details about fetching location data, see Configuring your app to use location services.

Configure the button’s content by specifying its icon and label styles. Customize its appearance using the cornerRadius and fontSize properties, or the standard view appearance properties backgroundColor and tintColor. For design guidance, see Human Interface Guidelines.

## Topics

### Customizing the icon style

var icon: CLLocationButtonIcon

The style of the location arrow icon on the button.

### Customizing the label text

var label: CLLocationButtonLabel

The text of the button label.

### Customizing the button appearance

var cornerRadius: CGFloat

The corner radius of the button.

var fontSize: CGFloat

The font size of the text on the button.

## Relationships

### Inherits From

- UIControl

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- NSTouchBarProvider
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UIContextMenuInteractionDelegate
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Location authorization

Sharing Your Location to Find a Park

Ask for location access using a customizable location button.

struct LocationButton

A SwiftUI button that grants one-time location authorization.

