

- SwiftUI
- AlertScene
-  init(\_:isPresented:presenting:actions:message:) 

Initializer

# init(\_:isPresented:presenting:actions:message:)

Creates an alert scene, using the given data to produce the alert’s content with a title, a set of actions, and a message. Note that this creates a text view on your behalf.

macOS 15.0+

``` source
init(
    _ title: S,
    isPresented: Binding,
    presenting data: T?,
    @ViewBuilder actions: (T) -> Actions,
    @ViewBuilder message: (T) -> Message
) where S : StringProtocol
```

Show all declarations

## Parameters 

`title`  

A text string used as the title of the alert.

`isPresented`  

A binding to a Boolean value that determines whether to present the alert. When the user presses or taps one of the alert’s actions, the system sets this value to `false` and dismisses.

`data`  

A source of truth that is passed to the alert to populate the message and actions.

`actions`  

A view builder returning the actions for the dialog.

`message`  

A view builder returning the message for the dialog.

