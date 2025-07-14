

- SwiftUI
- AlertScene
-  init(\_:isPresented:actions:) 

Initializer

# init(\_:isPresented:actions:)

Creates an alert scene with a title and a set of actions.

macOS 15.0+

``` source
init(
    _ title: Text,
    isPresented: Binding,
    @ViewBuilder actions: () -> Actions
) where Message == EmptyView
```

Show all declarations

## Parameters 

`title`  

The title of the alert.

`isPresented`  

A binding to a Boolean value that determines whether to present the alert. When the user presses or taps one of the alert’s actions, the system sets this value to `false` and dismisses.

`actions`  

A view builder returning the actions for the dialog.

