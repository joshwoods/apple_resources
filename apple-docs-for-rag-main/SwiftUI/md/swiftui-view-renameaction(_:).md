

- SwiftUI
- View
-  renameAction(\_:) 

Instance Method

# renameAction(\_:)

Sets a closure to run for the rename action.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func renameAction(_ action: @escaping () -> Void) -> some View
```

Show all declarations

## Parameters 

`action`  

A closure to run when renaming.

## Return Value

A view that has the specified rename action.

## Discussion

Use this modifier in conjunction with the RenameButton to implement standard rename interactions. A rename button receives its action from the environment. Use this modifier to customize the action provided to the rename button.

```
struct RowView: View {
    @State private var text = ""
    @FocusState private var isFocused: Bool

    var body: some View {
        TextField(text: $item.name) {
            Text("Prompt")
        }
        .focused($isFocused)
        .contextMenu {
            RenameButton()
            // ... your own custom actions
        }
        .renameAction { isFocused = true }
}
```

When the user taps the rename button in the context menu, the rename action focuses the text field by setting the `isFocused` property to true.

## See Also

### Renaming a document

struct RenameButton

A button that triggers a standard rename action.

var rename: RenameAction?

An action that activates the standard rename interaction.

struct RenameAction

An action that activates a standard rename interaction.

