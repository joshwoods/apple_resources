

- FamilyControls
- FamilyActivityPicker
-  alert(\_:isPresented:actions:) 

Instance Method

# alert(\_:isPresented:actions:)

Presents an alert when a given condition is true, using a text view for the title.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func alert(
    _ title: Text,
    isPresented: Binding,
    @ViewBuilder actions: () -> A
) -> some View where A : View
```

## Parameters 

`title`  

The title of the alert.

`isPresented`  

A binding to a Boolean value that determines whether to present the alert. When the user presses or taps one of the alert’s actions, the system sets this value to `false` and dismisses.

`actions`  

A `ViewBuilder` returning the alert’s actions.

## Discussion

In the example below, a login form conditionally presents an alert by setting the `didFail` state variable. When the form sets the value to to `true`, the system displays an alert with an “OK” action.

```
struct Login: View {
    @State private var didFail = false
    let alertTitle: String = "Login failed."

    var body: some View {
        LoginForm(didFail: $didFail)
            .alert(
                Text(alertTitle),
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

## See Also

### Alerts

func alert&lt;A>(LocalizedStringKey, isPresented: Binding&lt;Bool>, actions: () -> A) -> some View

Presents an alert when a given condition is true, using a localized string key for the title.

func alert&lt;S, A>(S, isPresented: Binding&lt;Bool>, actions: () -> A) -> some View

Presents an alert when a given condition is true, using a string variable as a title.

func alert&lt;S, A, T>(S, isPresented: Binding&lt;Bool>, presenting: T?, actions: (T) -> A) -> some View

Presents an alert using the given data to produce the alert’s content and a string variable as a title.

func alert&lt;A, T>(Text, isPresented: Binding&lt;Bool>, presenting: T?, actions: (T) -> A) -> some View

Presents an alert using the given data to produce the alert’s content and a text view as a title.

func alert&lt;A, T>(LocalizedStringKey, isPresented: Binding&lt;Bool>, presenting: T?, actions: (T) -> A) -> some View

Presents an alert using the given data to produce the alert’s content and a localized string key for a title.

func alert&lt;E, A>(isPresented: Binding&lt;Bool>, error: E?, actions: () -> A) -> some View

Presents an alert when an error is present.

