

- SwiftUI
- View
-  scenePadding(\_:) 

Instance Method

# scenePadding(\_:)

Adds padding to the specified edges of this view using an amount that’s appropriate for the current scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func scenePadding(_ edges: Edge.Set = .all) -> some View
```

## Parameters 

`edges`  

The set of edges along which to pad this view.

## Return Value

A view that’s padded on specified edges by a scene-appropriate amount.

## Discussion

Use this modifier to add a scene-appropriate amount of padding to a view. Specify either a single edge value from Edge.Set, or an OptionSet that describes the edges to pad.

In macOS, use scene padding to produce the recommended spacing around the root view of a window. In watchOS, use scene padding to align elements of your user interface with top level elements, like the title of a navigation view. For example, compare the effects of different kinds of padding on text views presented inside a NavigationView in watchOS:

```
VStack(alignment: .leading, spacing: 10) {
    Text("Scene padding")
        .scenePadding(.horizontal)
        .border(.red) // Border added for reference.
    Text("Regular padding")
        .padding(.horizontal)
        .border(.green)
    Text("Text with no padding")
        .border(.blue)
    Button("Button") { }
}
.navigationTitle("Hello World")
```

The text with scene padding automatically aligns with the title, unlike the text that uses the default padding or the text without padding:

Scene padding in watchOS also ensures that your content avoids the curved edges of a device like Apple Watch Series 7. In other platforms, scene padding produces the same default padding that you get from the padding(_:_:) modifier.

Important

Scene padding doesn’t pad the top and bottom edges of a view in watchOS, even if you specify those edges as part of the input. For example, if you specify vertical instead of horizontal in the example above, the modifier would have no effect in watchOS. It does, however, apply to all the edges that you specify in other platforms.

## See Also

### Adding padding around a view

func padding(_:)

Adds a different padding amount to each edge of this view.

func padding(Edge.Set, CGFloat?) -> some View

Adds an equal padding amount to specific edges of this view.

func padding3D(_:)

Pads this view using the edge insets you specify.

func padding3D(Edge3D.Set, CGFloat?) -> some View

Pads this view using the edge insets you specify.

func scenePadding(ScenePadding, edges: Edge.Set) -> some View

Adds a specified kind of padding to the specified edges of this view using an amount that’s appropriate for the current scene.

struct ScenePadding

The padding used to space a view from its containing scene.

