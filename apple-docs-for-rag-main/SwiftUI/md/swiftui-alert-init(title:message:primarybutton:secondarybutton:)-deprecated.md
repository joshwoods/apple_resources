

- SwiftUI
- Alert
-  init(title:message:primaryButton:secondaryButton:) Deprecated

Initializer

# init(title:message:primaryButton:secondaryButton:)

Creates an alert with two buttons.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
init(
    title: Text,
    message: Text? = nil,
    primaryButton: Alert.Button,
    secondaryButton: Alert.Button
)
```

Deprecated

Use a View modifier like alert(_:isPresented:presenting:actions:message:) instead.

## Parameters 

`title`  

The title of the alert.

`message`  

The message to display in the body of the alert.

`primaryButton`  

The first button to show in the alert.

`secondaryButton`  

The second button to show in the alert.

## Discussion

The system determines the visual ordering of the buttons.

## See Also

### Creating an alert

init(title: Text, message: Text?, dismissButton: Alert.Button?)

Creates an alert with one button.

Deprecated

static func sideBySideButtons(title: Text, message: Text?, primaryButton: Alert.Button, secondaryButton: Alert.Button) -> Alert

Creates a side by side button alert.

Deprecated

