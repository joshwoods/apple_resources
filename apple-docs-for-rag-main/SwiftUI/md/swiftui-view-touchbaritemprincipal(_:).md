

- SwiftUI
- View
-  touchBarItemPrincipal(\_:) 

Instance Method

# touchBarItemPrincipal(\_:)

Sets principal views that have special significance to this Touch Bar.

macOS 10.15+

``` source
nonisolated
func touchBarItemPrincipal(_ principal: Bool = true) -> some View
```

## Parameters 

`principal`  

A Boolean value that indicates whether to display this view prominently in the Touch Bar compared to other views.

## Return Value

A Touch Bar view with one element centered in the Touch Bar row.

## Discussion

Use `touchBarItemPrincipal(_:)` to designate a view as a significant view in the Touch Bar. Currently, that view will be placed in the center of the row.

The example below sets the last button as the principal button for the Touch Bar view.

```
let touchBarItems = TouchBar(id: "myBarItems") {
    Button("♣️", action: {})
    Button("♥️", action: {})
    Button("♠️", action: {})
    Button("♦️", action: {})
       .touchBarItemPrincipal(true)
}

TextField("TouchBar Demo", text: $placeholder)
    .frame(maxWidth: .infinity, maxHeight: .infinity)
    .focusable()
    .touchBar(touchBarItems)
```

Note

Multiple visible bars may each specify a principal view, but the system only honors one of them.

## See Also

### Managing Touch Bar input

func touchBar&lt;Content>(content: () -> Content) -> some View

Sets the content that the Touch Bar displays.

func touchBar&lt;Content>(TouchBar&lt;Content>) -> some View

Sets the Touch Bar content to be shown in the Touch Bar when applicable.

func touchBarCustomizationLabel(Text) -> some View

Sets a user-visible string that identifies the view’s functionality.

func touchBarItemPresence(TouchBarItemPresence) -> some View

Sets the behavior of the user-customized view.

struct TouchBar

A container for a view that you can show in the Touch Bar.

enum TouchBarItemPresence

Options that affect user customization of the Touch Bar.

