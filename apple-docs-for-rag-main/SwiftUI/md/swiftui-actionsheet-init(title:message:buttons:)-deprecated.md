

- SwiftUI
- ActionSheet
-  init(title:message:buttons:) Deprecated

Initializer

# init(title:message:buttons:)

Creates an action sheet with the provided buttons.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
init(
    title: Text,
    message: Text? = nil,
    buttons: [ActionSheet.Button] = [.cancel()]
)
```

Deprecated

Use a View modifier like confirmationDialog(_:isPresented:titleVisibility:presenting:actions:message:) instead.

## Parameters 

`title`  

The title of the action sheet.

`message`  

The message to display in the body of the action sheet.

`buttons`  

The buttons to show in the action sheet.

