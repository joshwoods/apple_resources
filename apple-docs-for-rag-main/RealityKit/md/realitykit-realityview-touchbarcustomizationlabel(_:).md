

- RealityKit
- RealityView
-  touchBarCustomizationLabel(\_:) 

Instance Method

# touchBarCustomizationLabel(\_:)

Sets a user-visible string that identifies the view’s functionality.

RealityKitSwiftUImacOS 10.15+

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

