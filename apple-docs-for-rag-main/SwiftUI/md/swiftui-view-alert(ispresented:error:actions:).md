

- SwiftUI
- View
-  alert(isPresented:error:actions:) 

Instance Method

# alert(isPresented:error:actions:)

Presents an alert when an error is present.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func alert(
    isPresented: Binding,
    error: E?,
    @ViewBuilder actions: () -> A
) -> some View where E : LocalizedError, A : View
```

## Parameters 

`isPresented`  

A binding to a Boolean value that determines whether to present the alert. When the user presses or taps one of the alert’s actions, the system sets this value to `false` and dismisses.

`error`  

An optional localized Error that is used to generate the alert’s title. The system passes the contents to the modifier’s closures. You use this data to populate the fields of an alert that you create that the system displays to the user.

`actions`  

A ViewBuilder returning the alert’s actions.

## Discussion

In the example below, a form conditionally presents an alert depending upon the value of an error. When the error value isn’t `nil`, the system presents an alert with an “OK” action.

The title of the alert is inferred from the error’s `errorDescription`.

```
struct TicketPurchase: View {
    @State private var error: TicketPurchaseError? = nil
    @State private var showAlert = false

    var body: some View {
        TicketForm(showAlert: $showAlert, error: $error)
            .alert(isPresented: $showAlert, error: error) {
                Button("OK") {
                    // Handle acknowledgement.
                }
            }
    }
}
```

All actions in an alert dismiss the alert after the action runs. The default button is shown with greater prominence. You can influence the default button by assigning it the defaultAction keyboard shortcut.

The system may reorder the buttons based on their role and prominence.

If no actions are present, the system includes a standard “OK” action. No default cancel action is provided. If you want to show a cancel action, use a button with a role of cancel.

On iOS, tvOS, and watchOS, alerts only support controls with labels that are Text. Passing any other type of view results in the content being omitted.

This modifier creates a Text view for the title on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See Text for more information about localizing strings.

## See Also

### Presenting an alert

struct AlertScene

A scene that renders itself as a standalone alert dialog.

func alert(_:isPresented:actions:)

Presents an alert when a given condition is true, using a text view for the title.

func alert(_:isPresented:presenting:actions:)

Presents an alert using the given data to produce the alert’s content and a text view as a title.

func alert(_:isPresented:actions:message:)

Presents an alert with a message when a given condition is true using a text view as a title.

func alert(_:isPresented:presenting:actions:message:)

Presents an alert with a message using the given data to produce the alert’s content and a text view for a title.

func alert&lt;E, A, M>(isPresented: Binding&lt;Bool>, error: E?, actions: (E) -> A, message: (E) -> M) -> some View

Presents an alert with a message when an error is present.

