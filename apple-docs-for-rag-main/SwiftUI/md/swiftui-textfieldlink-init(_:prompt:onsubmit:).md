

- SwiftUI
- TextFieldLink
-  init(\_:prompt:onSubmit:) 

Initializer

# init(\_:prompt:onSubmit:)

Creates a TextFieldLink which when pressed will request text input from the user.

watchOS 9.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    prompt: Text? = nil,
    onSubmit: @escaping (String) -> Void
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

A key for the TextFieldLink’s localized title, that describes the purpose of requesting text input.

`prompt`  

Text which describes the reason for requesting text input.

`onSubmit`  

An action to perform when text input has been accepted and dismissed

## See Also

### Creating a text field link

init(prompt: Text?, label: () -> Label, onSubmit: (String) -> Void)

Creates a TextFieldLink which when pressed will request text input from the user.

