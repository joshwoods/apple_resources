

- Assignables
- AssignedWorkDocumentView
-  confirmationDialog(\_:isPresented:titleVisibility:actions:) 

Instance Method

# confirmationDialog(\_:isPresented:titleVisibility:actions:)

Presents a confirmation dialog when a given condition is true, using a text view for the title.

AssignablesSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func confirmationDialog(
    _ title: Text,
    isPresented: Binding,
    titleVisibility: Visibility = .automatic,
    @ViewBuilder actions: () -> A
) -> some View where A : View
```

## Parameters 

`title`  

The title of the dialog.

`isPresented`  

A binding to a Boolean value that determines whether to present the dialog. When the user presses or taps the dialog’s default action button, the system sets this value to `false`, dismissing the dialog.

`titleVisibility`  

The visibility of the dialog’s title. The default value is `Visibility/automatic`.

`actions`  

A view builder returning the dialog’s actions.

## Discussion

In the example below, a button conditionally presents a confirmation dialog depending upon the value of a bound Boolean variable. When the Boolean value is set to `true`, the system displays a confirmation dialog with a cancel action and a destructive action.

```
struct ConfirmEraseItems: View {
    @State private var isShowingDialog = false
    var body: some View {
        Button("Empty Trash") {
            isShowingDialog = true
        }
        .confirmationDialog(
            Text("Permanently erase the items in the trash?"),
            isPresented: $isShowingDialog
        ) {
            Button("Empty Trash", role: .destructive) {
                // Handle empty trash action.
            }
        }
    }
}
```

All actions in a confirmation dialog will dismiss the dialog after the action runs. The default button will be shown with greater prominence. You can influence the default button by assigning it the `KeyboardShortcut/defaultAction` keyboard shortcut.

The system may reorder the buttons based on their role and prominence.

Dialogs include a standard dismiss action by default. If you provide a button with a role of `ButtonRole/cancel`, that button takes the place of the default dismiss action. You don’t have to dismiss the presentation with the cancel button’s action.

Note

In regular size classes in iOS, the system renders confirmation dialogs as a popover that the user dismisses by tapping anywhere outside the popover, rather than displaying the standard dismiss action.

