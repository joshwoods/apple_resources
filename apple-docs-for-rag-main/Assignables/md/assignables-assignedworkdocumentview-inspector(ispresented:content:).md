

- Assignables
- AssignedWorkDocumentView
-  inspector(isPresented:content:) 

Instance Method

# inspector(isPresented:content:)

Inserts an inspector at the applied position in the view hierarchy.

AssignablesSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
nonisolated
func inspector(
    isPresented: Binding,
    @ViewBuilder content: () -> V
) -> some View where V : View
```

## Parameters 

`isPresented`  

A binding to `Bool` controlling the presented state.

`content`  

The inspector content.

## Discussion

Apply this modifier to declare an inspector with a context-dependent presentation. For example, an inspector can present as a trailing column in a horizontally regular size class, but adapt to a sheet in a horizontally compact size class.

```
struct ShapeEditor: View {
    @State var presented: Bool = false
    var body: some View {
        MyEditorView()
            .inspector(isPresented: $presented) {
                TextTraitsInspectorView()
            }
    }
}
```

Note

Trailing column inspectors have their presentation state restored by the framework.

See Also

`InspectorCommands` for including the default inspector commands and keyboard shortcuts.

