

- SwiftUI
- AlertScene
-  init(\_:isPresented:actions:message:) 

Initializer

# init(\_:isPresented:actions:message:)

Creates an alert scene with a title, a set of actions, and a message.

macOS 15.0+

``` source
init(
    _ title: Text,
    isPresented: Binding,
    @ViewBuilder actions: () -> Actions,
    @ViewBuilder message: () -> Message
)
```

Show all declarations

## Parameters 

`title`  

The title of the alert.

`isPresented`  

A binding to a Boolean value that determines whether to present the alert. When the user presses or taps one of the alert’s actions, the system sets this value to `false` and dismisses.

`actions`  

A view builder returning the actions for the dialog.

`message`  

A view builder returning the message for the dialog.

