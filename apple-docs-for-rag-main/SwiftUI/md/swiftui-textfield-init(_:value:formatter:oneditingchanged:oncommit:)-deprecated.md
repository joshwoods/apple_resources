

- SwiftUI
- TextField
-  init(\_:value:formatter:onEditingChanged:onCommit:) Deprecated

Initializer

# init(\_:value:formatter:onEditingChanged:onCommit:)

Creates an instance which binds over an arbitrary type, `T`.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
init(
    _ title: S,
    value: Binding,
    formatter: Formatter,
    onEditingChanged: @escaping (Bool) -> Void,
    onCommit: @escaping () -> Void
) where S : StringProtocol
```

Available when `Label` is `Text`.

Deprecated

Use init(_:value:formatter:prompt:) instead. Add the onSubmit(of:_:) view modifier for the `onCommit` behavior. Use FocusState and focused(_:equals:) for the `onEditingChanged` behavior.

Show all declarations

## Parameters 

`title`  

The title of the text field, describing its purpose.

`value`  

The underlying value to be edited.

`formatter`  

A formatter to use when converting between the string the user edits and the underlying value of type `T`. In the event that `formatter` is unable to perform the conversion, `binding.value` isn’t modified.

`onEditingChanged`  

The action to perform when the user begins editing `text` and after the user finishes editing `text`. The closure receives a Boolean value that indicates the editing status: `true` when the user begins editing, `false` when they finish.

`onCommit`  

An action to perform when the user performs an action (for example, when the user presses the Return key) while the text field has focus.

## See Also

### Creating a text field with a value

init(_:value:formatter:onCommit:)

Create an instance which binds over an arbitrary type, `V`.

Deprecated

init(_:value:formatter:onEditingChanged:)

Create an instance which binds over an arbitrary type, `V`.

Deprecated

