

- SwiftUI
- TextField
-  init(\_:text:onEditingChanged:onCommit:) Deprecated

Initializer

# init(\_:text:onEditingChanged:onCommit:)

Creates a text field with a text label generated from a localized title string.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    text: Binding,
    onEditingChanged: @escaping (Bool) -> Void,
    onCommit: @escaping () -> Void
)
```

Available when `Label` is `Text`.

Deprecated

Use init(_:text:prompt:) instead. Add the onSubmit(of:_:) view modifier for the `onCommit` behavior. Use FocusState and focused(_:equals:) for the `onEditingChanged` behavior.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title of the text field, describing its purpose.

`text`  

The text to display and edit.

`onEditingChanged`  

The action to perform when the user begins editing `text` and after the user finishes editing `text`. The closure receives a Boolean value that indicates the editing status: `true` when the user begins editing, `false` when they finish.

`onCommit`  

An action to perform when the user performs an action (for example, when the user presses the Return key) while the text field has focus.

## See Also

### Creating a text field with a string

init(_:text:onCommit:)

Creates a text field with a text label generated from a localized title string.

Deprecated

init(_:text:onEditingChanged:)

Creates a text field with a text label generated from a localized title string.

Deprecated

