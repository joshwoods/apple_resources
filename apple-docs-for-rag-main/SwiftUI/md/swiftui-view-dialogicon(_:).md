

- SwiftUI
- View
-  dialogIcon(\_:) 

Instance Method

# dialogIcon(\_:)

Configures the icon used by dialogs within this view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 13.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
func dialogIcon(_ icon: Image?) -> some View
```

## Parameters 

`icon`  

The custom icon to use for confirmation dialogs and alerts. Passing `nil` will use the default app icon.

## Discussion

On macOS, this icon replaces the default icon of the app.

On watchOS, this icon will be shown in any dialogs presented.

This modifier has no effect on other platforms.

The following example configures a `confirmationDialog` with a custom image.

```
Button("Delete items") {
    isShowingDialog = true
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
.dialogIcon(Image(...))
```

## See Also

### Configuring a dialog

func dialogIcon(Image?) -> some Scene

Configures the icon used by alerts.

func dialogSeverity(DialogSeverity) -> some View

func dialogSeverity(DialogSeverity) -> some Scene

Sets the severity for alerts.

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some View

Enables user suppression of dialogs and alerts presented within `self`, with a default suppression message on macOS. Unused on other platforms.

func dialogSuppressionToggle(isSuppressed: Binding&lt;Bool>) -> some Scene

Enables user suppression of an alert with a custom suppression message.

func dialogSuppressionToggle(_:isSuppressed:)

Enables user suppression of dialogs and alerts presented within `self`, with a custom suppression message on macOS. Unused on other platforms.

