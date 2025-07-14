

- SwiftUI
- AlertScene
-  init(\_:isPresented:presenting:actions:) 

Initializer

# init(\_:isPresented:presenting:actions:)

Creates an alert scene, using the given data to produce the alert’s content with a title, and a set of actions. Note that this creates a text view on your behalf.

macOS 15.0+

``` source
init(
    _ title: S,
    isPresented: Binding,
    presenting data: T?,
    @ViewBuilder actions: (T) -> Actions
) where Message == EmptyView, S : StringProtocol
```

Show all declarations

## Parameters 

`title`  

The title of the alert.

`isPresented`  

A binding to a Boolean value that determines whether to present the alert. When the user presses or taps one of the alert’s actions, the system sets this value to `false` and dismisses.

`data`  

A source of truth that is passed to the alert to populate the message and actions.

`actions`  

A view builder returning the actions for the dialog.

