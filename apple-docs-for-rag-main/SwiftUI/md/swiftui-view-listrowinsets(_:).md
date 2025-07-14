

- SwiftUI
- View
-  listRowInsets(\_:) 

Instance Method

# listRowInsets(\_:)

Applies an inset to the rows in a list.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func listRowInsets(_ insets: EdgeInsets?) -> some View
```

## Parameters 

`insets`  

The EdgeInsets to apply to the edges of the view.

## Return Value

A view that uses the given edge insets when used as a list cell.

## Discussion

Use `listRowInsets(_:)` to change the default padding of the content of list items.

In the example below, the `Flavor` enumeration provides content for list items. The SwiftUI ForEach structure computes views for each element of the `Flavor` enumeration and extracts the raw value of each of its elements using the resulting text to create each list row item. The `listRowInsets(_:)` modifier then changes the edge insets of each row of the list according to the EdgeInsets provided:

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
                    .listRowInsets(.init(top: 0,
                                         leading: 25,
                                         bottom: 0,
                                         trailing: 0))
            }
        }
    }
}
```

## See Also

### Configuring rows

func listRowHoverEffect(HoverEffect?) -> some View

Requests that the containing list row use the provided hover effect.

func listRowHoverEffectDisabled(Bool) -> some View

Requests that the containing list row have its hover effect disabled.

func listItemTint(_:)

Sets a fixed tint color for content in a list.

struct ListItemTint

A tint effect configuration that you can apply to content in a list.

var defaultMinListRowHeight: CGFloat

The default minimum height of a row in a `List`. The default minimum height of a row in a list.

