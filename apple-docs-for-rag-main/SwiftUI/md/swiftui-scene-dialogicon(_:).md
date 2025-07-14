

- SwiftUI
- Scene
-  dialogIcon(\_:) 

Instance Method

# dialogIcon(\_:)

Configures the icon used by alerts.

macOS 15.0+

``` source
nonisolated
func dialogIcon(_ icon: Image?) -> some Scene
```

## Parameters 

`icon`  

The custom icon to use for the alert. Passing `nil` will use the default app icon.

## Discussion

In macOS, this icon replaces the default icon of the app.

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
        .dialogIcon(Image(Trash.png))
    }
}
```

## See Also

### Configuring a dialog

func dialogIcon(Image?) -> some View

Configures the icon used by dialogs within this view.

func dialogSeverity(DialogSeverity) -> some View

func dialogSeverity(DialogSeverity) -> some Scene

Sets the severity for alerts.

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some View

Enables user suppression of dialogs and alerts presented within `self`, with a default suppression message on macOS. Unused on other platforms.

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some Scene

Enables user suppression of an alert with a custom suppression message.

func dialogSuppressionToggle(_:isSuppressed:)

Enables user suppression of dialogs and alerts presented within `self`, with a custom suppression message on macOS. Unused on other platforms.

