

- RealityKit
- RealityViewDefaultPlaceholder
-  touchBar(\_:) 

Instance Method

# touchBar(\_:)

Sets the Touch Bar content to be shown in the Touch Bar when applicable.

RealityKitSwiftUImacOS 10.15+

``` source
nonisolated
func touchBar(_ touchBar: TouchBar) -> some View where Content : View
```

## Parameters 

`touchBar`  

A collection of views that the Touch Bar displays.

## Return Value

A view that contains the Touch Bar content.

## Discussion

Use `View/touchBar(_:)` to provide a static set of views that are displayed by the Touch Bar when appropriate, depending on whether the view has focus.

The example below provides Touch Bar content in-line, that creates the content the Touch Bar displays:

```
func selectHearts() {/* ... */ }
func selectClubs() { /* ... */ }
func selectSpades() { /* ... */ }
func selectDiamonds() { /* ... */ }

TextField("TouchBar Demo", text: $placeholder)
    .frame(maxWidth: .infinity, maxHeight: .infinity)
    .focusable()
    .touchBar {
        Button("♥️ - Hearts", action: selectHearts)
        Button("♣️ - Clubs", action: selectClubs)
        Button("♠️ - Spades", action: selectSpades)
        Button("♦️ - Diamonds", action: selectDiamonds)
    }
```

