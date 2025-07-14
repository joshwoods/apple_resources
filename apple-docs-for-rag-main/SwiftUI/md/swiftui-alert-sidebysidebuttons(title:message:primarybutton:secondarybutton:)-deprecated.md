

- SwiftUI
- Alert
-  sideBySideButtons(title:message:primaryButton:secondaryButton:) Deprecated

Type Method

# sideBySideButtons(title:message:primaryButton:secondaryButton:)

Creates a side by side button alert.

watchOS 6.0–11.4Deprecated

``` source
static func sideBySideButtons(
    title: Text,
    message: Text? = nil,
    primaryButton: Alert.Button,
    secondaryButton: Alert.Button
) -> Alert
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

init(title: Text, message: Text?, primaryButton: Alert.Button, secondaryButton: Alert.Button)

Creates an alert with two buttons.

Deprecated

