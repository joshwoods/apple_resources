

- Assignables
- AssignableDocumentView
-  dialogIcon(\_:) 

Instance Method

# dialogIcon(\_:)

Configures the icon used by dialogs within this view.

AssignablesSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 13.0+tvOS 17.0+watchOS 10.0+

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

