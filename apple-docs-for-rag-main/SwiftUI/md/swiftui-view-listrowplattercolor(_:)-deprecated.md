

- SwiftUI
- View
-  listRowPlatterColor(\_:) Deprecated

Instance Method

# listRowPlatterColor(\_:)

Sets the color that the system applies to the row background when this view is placed in a list.

watchOS 6.0–11.4Deprecated

``` source
nonisolated
func listRowPlatterColor(_ color: Color?) -> some View
```

Deprecated

Use listItemTint(_:) instead.

## Parameters 

`color`  

The Color to apply to the system cell.

## Return Value

A view with the specified `color` applied to the system cell.

## Discussion

Use `listRowPlatterColor(_:)` to set the underlying row background color in a list.

In the example below, the `Flavor` enumeration provides content for list items. The SwiftUI List builder iterates over the `Flavor` enumeration and extracts the raw value of each of its elements using the resulting text to create each list row item. After the list builder finishes, the `listRowPlatterColor(_:)` modifier sets the underlying row background color to the Color you specify.

```
struct ContentView: View {
    enum Flavor: String, CaseIterable, Identifiable {
        var id: String { self.rawValue }
        case vanilla, chocolate, strawberry
    }

    var body: some View {
        List {
            ForEach(Flavor.allCases) {
                Text($0.rawValue)
                    .listRowPlatterColor(.green)
            }
        }
    }
}
```

## See Also

### Appearance modifiers

func colorScheme(ColorScheme) -> some View

Sets this view’s color scheme.

Deprecated

func background&lt;Background>(Background, alignment: Alignment) -> some View

Layers the given view behind this view.

Deprecated

func overlay&lt;Overlay>(Overlay, alignment: Alignment) -> some View

Layers a secondary view in front of this view.

Deprecated

func foregroundColor(Color?) -> some View

Sets the color of the foreground elements displayed by this view.

Deprecated

func complicationForeground() -> some View

Promotes this view to the foreground in a complication.

Deprecated

