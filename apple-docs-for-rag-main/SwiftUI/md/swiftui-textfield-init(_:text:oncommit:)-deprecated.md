

- SwiftUI
- TextField
-  init(\_:text:onCommit:) Deprecated

Initializer

# init(\_:text:onCommit:)

Creates a text field with a text label generated from a localized title string.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    text: Binding,
    onCommit: @escaping () -> Void
)
```

Available when `Label` is `Text`.

Deprecated

Renamed TextField.init(\_:text:onEditingChanged:). Use View.onSubmit(of:\_:) for functionality previously provided by the onCommit parameter. Use FocusState\ and View.focused(\_:equals:) for functionality previously provided by the onEditingChanged parameter.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title of the text field, describing its purpose.

`text`  

The text to display and edit.

`onCommit`  

An action to perform when the user performs an action (for example, when the user presses the Return key) while the text field has focus.

## See Also

### Creating a text field with a string

init(_:text:onEditingChanged:onCommit:)

Creates a text field with a text label generated from a localized title string.

Deprecated

init(_:text:onEditingChanged:)

Creates a text field with a text label generated from a localized title string.

Deprecated

