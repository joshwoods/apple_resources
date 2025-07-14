

- SwiftUI
- Scene
-  dialogSeverity(\_:) 

Instance Method

# dialogSeverity(\_:)

Sets the severity for alerts.

macOS 15.0+

``` source
nonisolated
func dialogSeverity(_ severity: DialogSeverity) -> some Scene
```

## Parameters 

`severity`  

The severity to use for alerts.

## Discussion

The following example configures an alert for erasing some number of items. Since this operation is destructive and non-recoverable, a `.critical` severity is used.

```
struct MyApp: App {
    @State private var isShowingDialog = false

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
        .dialogSeverity(.critical)
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

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some View

Enables user suppression of dialogs and alerts presented within `self`, with a default suppression message on macOS. Unused on other platforms.

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some Scene

Enables user suppression of an alert with a custom suppression message.

func dialogSuppressionToggle(_:isSuppressed:)

Enables user suppression of dialogs and alerts presented within `self`, with a custom suppression message on macOS. Unused on other platforms.

