

- SwiftUI
- Alert
-  init(title:message:dismissButton:) Deprecated

Initializer

# init(title:message:dismissButton:)

Creates an alert with one button.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
init(
    title: Text,
    message: Text? = nil,
    dismissButton: Alert.Button? = nil
)
```

Deprecated

Use a View modifier like alert(_:isPresented:presenting:actions:message:) instead.

## Parameters 

`title`  

The title of the alert.

`message`  

The message to display in the body of the alert.

`dismissButton`  

The button that dismisses the alert.

## See Also

### Creating an alert

init(title: Text, message: Text?, primaryButton: Alert.Button, secondaryButton: Alert.Button)

Creates an alert with two buttons.

Deprecated

static func sideBySideButtons(title: Text, message: Text?, primaryButton: Alert.Button, secondaryButton: Alert.Button) -> Alert

Creates a side by side button alert.

Deprecated

