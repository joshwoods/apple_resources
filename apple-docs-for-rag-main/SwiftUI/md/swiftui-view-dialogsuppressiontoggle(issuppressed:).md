

- SwiftUI
- View
-  dialogSuppressionToggle(isSuppressed:) 

Instance Method

# dialogSuppressionToggle(isSuppressed:)

Enables user suppression of dialogs and alerts presented within `self`, with a default suppression message on macOS. Unused on other platforms.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func dialogSuppressionToggle(isSuppressed: Binding) -> some View
```

## Parameters 

`isSuppressed`  

Whether the suppression toggle is on or off in the dialog.

## Discussion

Applying dialog suppression adds a toggle to dialogs on macOS, which allows the user to request the alert not be displayed again. Typically whether a dialog is suppressed is stored in `AppStorage` and used to decide whether to present the dialog in the future.

The following example configures a `confirmationDialog` with a suppression toggle. The toggle’s state is stored in `AppStorage` and used to determine whether or not to show the dialog when the “Delete Items” button is pressed.

```
struct ConfirmEraseItems: View {
    @State private var isShowingDialog = false

    @AppStorage("suppressEraseItemAlert")
    private var suppressAlert = false

    var body: some View {
        Button("Delete Items") {
            if !suppressAlert {
                isShowingDialog = true
            } else {
                // Handle item deletion.
            }
        }
        .confirmationDialog(
            "Are you sure you want to erase these items?",
            isPresented: $isShowingDialog
        ) {
            Button("Erase", role: .destructive) {
                // Handle item deletion.
            }
            Button("Cancel", role: .cancel) {
                isShowingDialog = false
            }
        }
        .dialogSuppressionToggle(isSuppressed: $suppressAlert)
    }
}
```

## See Also

### Configuring a dialog

func dialogIcon(Image?) -> some View

Configures the icon used by dialogs within this view.

func dialogIcon(Image?) -> some Scene

Configures the icon used by alerts.

func dialogSeverity(DialogSeverity) -> some View

func dialogSeverity(DialogSeverity) -> some Scene

Sets the severity for alerts.

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some Scene

Enables user suppression of an alert with a custom suppression message.

func dialogSuppressionToggle(_:isSuppressed:)

Enables user suppression of dialogs and alerts presented within `self`, with a custom suppression message on macOS. Unused on other platforms.

