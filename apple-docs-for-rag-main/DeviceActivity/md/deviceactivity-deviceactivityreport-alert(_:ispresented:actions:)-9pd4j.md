

- DeviceActivity
- DeviceActivityReport
-  alert(\_:isPresented:actions:) 

Instance Method

# alert(\_:isPresented:actions:)

Presents an alert when a given condition is true, using a localized string key for the title.

DeviceActivitySwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func alert(
    _ titleKey: LocalizedStringKey,
    isPresented: Binding,
    @ViewBuilder actions: () -> A
) -> some View where A : View
```

## Parameters 

`titleKey`  

The key for the localized string that describes the title of the alert.

`isPresented`  

A binding to a Boolean value that determines whether to present the alert. When the user presses or taps one of the alert’s actions, the system sets this value to `false` and dismisses.

`actions`  

A `ViewBuilder` returning the alert’s actions.

## Discussion

In the example below, a login form conditionally presents an alert by setting the `didFail` state variable. When the form sets the value to to `true`, the system displays an alert with an “OK” action.

```
struct Login: View {
    @State private var didFail = false

    var body: some View {
        LoginForm(didFail: $didFail)
            .alert(
                "Login failed.",
                isPresented: $didFail
            ) {
                Button("OK") {
                    // Handle the acknowledgement.
                }
            }
    }
}
```

All actions in an alert dismiss the alert after the action runs. The default button is shown with greater prominence. You can influence the default button by assigning it the `KeyboardShortcut/defaultAction` keyboard shortcut.

The system may reorder the buttons based on their role and prominence.

If no actions are present, the system includes a standard “OK” action. No default cancel action is provided. If you want to show a cancel action, use a button with a role of `ButtonRole/cancel`.

On iOS, tvOS, and watchOS, alerts only support controls with labels that are `Text`. Passing any other type of view results in the content being omitted.

This modifier creates a `Text` view for the title on your behalf, and treats the localized key similar to `Text/init(_:tableName:bundle:comment:)`. See `Text` for more information about localizing strings.

