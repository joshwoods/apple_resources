

- RealityKit
- RealityViewDefaultPlaceholder
-  inspectorColumnWidth(min:ideal:max:) 

Instance Method

# inspectorColumnWidth(min:ideal:max:)

Sets a flexible, preferred width for the inspector in a trailing-column presentation.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+

``` source
nonisolated
func inspectorColumnWidth(
    min: CGFloat? = nil,
    ideal: CGFloat,
    max: CGFloat? = nil
) -> some View
```

## Parameters 

`min`  

The minimum allowed width for the trailing column inspector

`ideal`  

The initial width of the inspector in the absence of state restoration. `ideal` influences the resulting width on macOS when a user double-clicks the divider on the leading edge of the inspector. clicks a divider to readjust

`max`  

The maximum allowed width for the trailing column inspector

## Discussion

Apply this modifier on the content of a `View/inspector(isPresented:content:)` to specify a preferred flexible width for the column. Use `View/inspectorColumnWidth(_:)` if you need to specify a fixed width.

The following example shows an editor interface with an inspector, which when presented as a trailing-column, has a preferred width of 225 points, maximum of 400, and a minimum of 150 at which point it will collapse, if allowed.

```
MyEditorView()
    .inspector {
        TextTraitsInspectorView()
            .inspectorColumnWidth(min: 150, ideal: 225, max: 400)
    }
```

Only some platforms enable flexible inspector columns. If you specify a width that the current presentation environment doesn’t support, SwiftUI may use a different width for your column.

