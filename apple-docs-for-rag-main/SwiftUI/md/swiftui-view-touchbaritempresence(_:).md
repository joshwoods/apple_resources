

- SwiftUI
- View
-  touchBarItemPresence(\_:) 

Instance Method

# touchBarItemPresence(\_:)

Sets the behavior of the user-customized view.

macOS 10.15+

``` source
nonisolated
func touchBarItemPresence(_ presence: TouchBarItemPresence) -> some View
```

## Parameters 

`presence`  

One of the allowed TouchBarItemPresence descriptions.

## Return Value

A trait that describes the behavior for this Touch Bar view.

## Discussion

Use `touchBarItemPresence(_:)` to define the visibility requirements of a particular Touch Bar view during customization by the user.

Touch Bar views may be:

- `.required`: not allowed to be removed by the user.

- `.default`: shown by default prior to user customization, but removable.

- `.optional`: not visible by default, but can be added through the customization palette.

Each TouchBarItemPresence must be initialized with a string that is a globally unique identifier for this item.

In the example below, all of the Touch Bar items are visible in the Touch Bar by default, except for the “Clubs” item. It’s set to `.optional` but is configurable by the user:

```
TextField("TouchBar Demo", text: $placeholder)
    .frame(maxWidth: .infinity, maxHeight: .infinity)
    .focusable()
    .touchBar {
        Button("♥️", action: selectHearts)
            .touchBarItemPresence(.required("heartsKey"))
        Button("♣️", action: selectClubs)
            .touchBarItemPresence(.optional("clubsKey"))
        Button("♠️", action: selectSpades)
            .touchBarItemPresence(.required("spadesKey"))
        Button("♦️", action: selectDiamonds)
            .touchBarItemPresence(.required("diamondsKey"))
}
```

## See Also

### Managing Touch Bar input

func touchBar&lt;Content>(content: () -> Content) -> some View

Sets the content that the Touch Bar displays.

func touchBar&lt;Content>(TouchBar&lt;Content>) -> some View

Sets the Touch Bar content to be shown in the Touch Bar when applicable.

func touchBarItemPrincipal(Bool) -> some View

Sets principal views that have special significance to this Touch Bar.

func touchBarCustomizationLabel(Text) -> some View

Sets a user-visible string that identifies the view’s functionality.

struct TouchBar

A container for a view that you can show in the Touch Bar.

enum TouchBarItemPresence

Options that affect user customization of the Touch Bar.

