

- FamilyControls
- FamilyActivityPicker
-  listRowBackground(\_:) 

Instance Method

# listRowBackground(\_:)

Places a custom background view behind a list row item.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func listRowBackground(_ view: V?) -> some View where V : View
```

## Parameters 

`view`  

The `View` to use as the background behind the list row view.

## Return Value

A list row view with `view` as its background view.

## Discussion

Use `listRowBackground(_:)` to place a custom background view behind a list row item.

In the example below, the `Flavor` enumeration provides content for list items. The SwiftUI `ForEach` structure computes views for each element of the `Flavor` enumeration and extracts the raw value of each of its elements using the resulting text to create each list row item. The `listRowBackground(_:)` modifier then places the view you supply behind each of the list row items:

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
                    .listRowBackground(Ellipse()
                                        .background(Color.clear)
                                        .foregroundColor(.purple)
                                        .opacity(0.3)
                    )
            }
        }
    }
}
```

## See Also

### Background Elements

func border&lt;S>(S, width: CGFloat) -> some View

Adds a border to this view with the specified style and width.

func background(ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to the default background style.

func background&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to a style.

func background&lt;S>(in: S, fillStyle: FillStyle) -> some View

Sets the view’s background to a shape filled with the default background style.

func background&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Sets the view’s background to a shape filled with a style.

func background&lt;S>(in: S, fillStyle: FillStyle) -> some View

Sets the view’s background to an insettable shape filled with the default background style.

func background&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Sets the view’s background to an insettable shape filled with a style.

