

- SwiftUI
- Scene
-  dialogSuppressionToggle(\_:isSuppressed:) 

Instance Method

# dialogSuppressionToggle(\_:isSuppressed:)

Enables user suppression of an alert with a custom suppression message.

macOS 15.0+

``` source
nonisolated
func dialogSuppressionToggle(
    _ label: Text,
    isSuppressed: Binding
) -> some Scene
```

Show all declarations

## Parameters 

`label`  

The label of the suppression toggle in the dialog. This parameter can be elided to use the default suppression title.

`isSuppressed`  

Whether the suppression toggle is on or off in the dialog.

## Discussion

Applying dialog suppression adds a toggle to dialogs on macOS, which allows the user to request the alert not be displayed again. Typically whether a dialog is suppressed is stored in `AppStorage` and used to decide whether to present the dialog in the future.

The following example configures an alert with a suppression toggle. The toggle’s state is stored in `AppStorage` and used to determine whether or not to show the dialog when the “Delete Items” button is pressed.

```
struct MyApp: App {
    @State private var isShowingDialog = false
    @AppStorage("suppressEraseItemAlert")
    private var suppressAlert = false

    var body: some Scene {
        Window(...) {
            Button("Delete items") {
                isShowingDialog = true
            }
        }

        AlertScene(
            "Are you sure you want to erase these items?",
            isPresented: $isShowingDialog
        ) {
            Button("Erase", role: .destructive) {
                // Handle item deletion.
            }
            Button("Cancel", role: .cancel) {
                // Handle cancellation
            }
        }
        .dialogSuppressionToggle(
            "Do not ask about erasing items again",
            isSuppressed: $suppressAlert)
    }
}
```

## See Also

### Interacting with dialogs

func dialogIcon(Image?) -> some Scene

Configures the icon used by alerts.

func dialogSeverity(DialogSeverity) -> some Scene

Sets the severity for alerts.

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some Scene

Enables user suppression of an alert with a custom suppression message.

