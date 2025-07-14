

- RealityKit
- Model3D
-  alert(\_:isPresented:actions:message:) 

Instance Method

# alert(\_:isPresented:actions:message:)

Presents an alert with a message when a given condition is true using a string variable as a title.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func alert(
    _ title: S,
    isPresented: Binding,
    @ViewBuilder actions: () -> A,
    @ViewBuilder message: () -> M
) -> some View where S : StringProtocol, A : View, M : View
```

## Parameters 

`title`  

A text string used as the title of the alert.

`isPresented`  

A binding to a Boolean value that determines whether to present the alert. When the user presses or taps one of the alert’s actions, the system sets this value to `false` and dismisses.

`actions`  

A `ViewBuilder` returning the alert’s actions.

`message`  

A `ViewBuilder` returning the message for the alert.

## Discussion

In the example below, a login form conditionally presents an alert by setting the `didFail` state variable. When the form sets the value to to `true`, the system displays an alert with an “OK” action.

```
struct Login: View {
    @State private var didFail = false
    let alertTitle: String = "Login failed."

    var body: some View {
        LoginForm(didFail: $didFail)
            .alert(
                alertTitle,
                isPresented: $didFail
            ) {
                Button("OK") {
                    // Handle the acknowledgement.
                }
            } message: {
                Text("Please check your credentials and try again.")
            }
    }
}
```

All actions in an alert dismiss the alert after the action runs. The default button is shown with greater prominence. You can influence the default button by assigning it the `KeyboardShortcut/defaultAction` keyboard shortcut.

The system may reorder the buttons based on their role and prominence.

If no actions are present, the system includes a standard “OK” action. No default cancel action is provided. If you want to show a cancel action, use a button with a role of `ButtonRole/cancel`.

On iOS, tvOS, and watchOS, alerts only support controls with labels that are `Text`. Passing any other type of view results in the content being omitted.

Only unstyled text is supported for the message.

