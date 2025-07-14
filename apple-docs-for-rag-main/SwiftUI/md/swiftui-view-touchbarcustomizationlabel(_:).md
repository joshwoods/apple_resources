

- SwiftUI
- View
-  touchBarCustomizationLabel(\_:) 

Instance Method

# touchBarCustomizationLabel(\_:)

Sets a user-visible string that identifies the view’s functionality.

macOS 10.15+

``` source
nonisolated
func touchBarCustomizationLabel(_ label: Text) -> some View
```

## Parameters 

`label`  

A `Text` view containing the customization label.

## Return Value

A Touch Bar element with a set customization label.

## Discussion

This string is visible during user customization.

```
TextField("TouchBar Demo", text: $placeholder)
    .frame(maxWidth: .infinity, maxHeight: .infinity)
    .focusable()
    .touchBar {
        Button("♥️", action: selectHearts)
            .touchBarCustomizationLabel(Text("Hearts"))
        Button("♣️", action: selectClubs)
            .touchBarCustomizationLabel(Text("Clubs"))
        Button("♠️", action: selectSpades)
            .touchBarCustomizationLabel(Text("Spades"))
        Button("♦️", action: selectDiamonds)
            .touchBarCustomizationLabel(Text("Diamonds"))
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

func touchBarItemPresence(TouchBarItemPresence) -> some View

Sets the behavior of the user-customized view.

struct TouchBar

A container for a view that you can show in the Touch Bar.

enum TouchBarItemPresence

Options that affect user customization of the Touch Bar.

