

- SwiftUI
- SecureField
-  init(\_:text:onCommit:) Deprecated

Initializer

# init(\_:text:onCommit:)

Creates an instance.

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

Use init(_:text:prompt:) instead. Add the onSubmit(of:_:) view modifier for the `onCommit` behavior.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title of `self`, describing its purpose.

`text`  

The text to display and edit.

`onCommit`  

The action to perform when the user performs an action (usually pressing the Return key) while the secure field has focus.

