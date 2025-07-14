

- FamilyControls
- FamilyActivityPicker
-  inspectorColumnWidth(\_:) 

Instance Method

# inspectorColumnWidth(\_:)

Sets a fixed, preferred width for the inspector containing this view when presented as a trailing column.

FamilyControlsSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
nonisolated
func inspectorColumnWidth(_ width: CGFloat) -> some View
```

## Parameters 

`width`  

The preferred fixed width for the inspector if presented as a trailing column.

## Discussion

Apply this modifier on the content of a `View/inspector(isPresented:content:)` to specify a fixed preferred width for the trailing column. Use `View/inspectorColumnWidth(min:ideal:max:)` if you need to specify a flexible width.

The following example shows an editor interface with an inspector, which when presented as a trailing-column, has a fixed width of 225 points. The example also uses `View/interactiveDismissDisabled(_:)` to prevent the inspector from being collapsed by user action like dragging a divider.

```
MyEditorView()
    .inspector {
        TextTraitsInspectorView()
            .inspectorColumnWidth(225)
            .interactiveDismissDisabled()
    }
```

Note

A fixed width does not prevent the user collapsing the inspector on macOS. See `View/interactiveDismissDisabled(_:)`.

