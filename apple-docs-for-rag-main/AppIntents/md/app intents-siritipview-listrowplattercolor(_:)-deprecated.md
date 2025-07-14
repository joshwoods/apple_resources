

- App Intents
- SiriTipView
-  listRowPlatterColor(\_:) Deprecated

Instance Method

# listRowPlatterColor(\_:)

Sets the color that the system applies to the row background when this view is placed in a list.

AppIntentsSwiftUIwatchOS 6.0–9.0Deprecated

``` source
nonisolated
func listRowPlatterColor(_ color: Color?) -> some View
```

## Parameters 

`color`  

The `Color` to apply to the system cell.

## Return Value

A view with the specified `color` applied to the system cell.

## Discussion

Use `View/listRowPlatterColor(_:)` to set the underlying row background color in a list.

In the example below, the `Flavor` enumeration provides content for list items. The SwiftUI `List` builder iterates over the `Flavor` enumeration and extracts the raw value of each of its elements using the resulting text to create each list row item. After the list builder finishes, the `listRowPlatterColor(_:)` modifier sets the underlying row background color to the `Color` you specify.

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

