

- SwiftUI
- TextFieldLink
-  init(prompt:label:onSubmit:) 

Initializer

# init(prompt:label:onSubmit:)

Creates a TextFieldLink which when pressed will request text input from the user.

watchOS 9.0+

``` source
nonisolated
init(
    prompt: Text? = nil,
    @ViewBuilder label: () -> Label,
    onSubmit: @escaping (String) -> Void
)
```

Available when `Label` conforms to `View`.

## Parameters 

`prompt`  

Text which describes the reason for requesting text input.

`label`  

A view that describes the action of requesting text input.

`onSubmit`  

An action to perform when text input has been accepted and dismissed

## See Also

### Creating a text field link

init(_:prompt:onSubmit:)

Creates a TextFieldLink which when pressed will request text input from the user.

