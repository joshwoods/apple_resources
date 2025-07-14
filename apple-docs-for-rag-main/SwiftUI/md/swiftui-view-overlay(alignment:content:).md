

- SwiftUI
- View
-  overlay(alignment:content:) 

Instance Method

# overlay(alignment:content:)

Layers the views that you specify in front of this view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func overlay(
    alignment: Alignment = .center,
    @ViewBuilder content: () -> V
) -> some View where V : View
```

## Parameters 

`alignment`  

The alignment that the modifier uses to position the implicit ZStack that groups the foreground views. The default is center.

`content`  

A ViewBuilder that you use to declare the views to draw in front of this view, stacked in the order that you list them. The last view that you list appears at the front of the stack.

## Return Value

A view that uses the specified content as a foreground.

## Discussion

Use this modifier to place one or more views in front of another view. For example, you can place a group of stars on a RoundedRectangle:

```
RoundedRectangle(cornerRadius: 8)
    .frame(width: 200, height: 100)
    .overlay(alignment: .topLeading) { Star(color: .red) }
    .overlay(alignment: .topTrailing) { Star(color: .yellow) }
    .overlay(alignment: .bottomLeading) { Star(color: .green) }
    .overlay(alignment: .bottomTrailing) { Star(color: .blue) }
```

The example above assumes that you’ve defined a `Star` view with a parameterized color:

```
struct Star: View {
    var color = Color.yellow

    var body: some View {
        Image(systemName: "star.fill")
            .foregroundStyle(color)
    }
}
```

By setting different `alignment` values for each modifier, you make the stars appear in different places on the rectangle:

If you specify more than one view in the `content` closure, the modifier collects all of the views in the closure into an implicit ZStack, taking them in order from back to front. For example, you can place a star and a Circle on a field of blue:

```
Color.blue
    .frame(width: 200, height: 200)
    .overlay {
        Circle()
            .frame(width: 100, height: 100)
        Star()
    }
```

Both the overlay modifier and the implicit ZStack composed from the overlay content — the circle and the star — use a default center alignment. The star appears centered on the circle, and both appear as a composite view centered in front of the square:

If you specify an alignment for the overlay, it applies to the implicit stack rather than to the individual views in the closure. You can see this if you add the bottom alignment:

```
Color.blue
    .frame(width: 200, height: 200)
    .overlay(alignment: .bottom) {
        Circle()
            .frame(width: 100, height: 100)
        Star()
    }
```

The circle and the star move down as a unit to align the stack’s bottom edge with the bottom edge of the square, while the star remains centered on the circle:

To control the placement of individual items inside the `content` closure, either use a different overlay modifier for each item, as the earlier example of stars in the corners of a rectangle demonstrates, or add an explicit ZStack inside the content closure with its own alignment:

```
Color.blue
    .frame(width: 200, height: 200)
    .overlay(alignment: .bottom) {
        ZStack(alignment: .bottom) {
            Circle()
                .frame(width: 100, height: 100)
            Star()
        }
    }
```

The stack alignment ensures that the star’s bottom edge aligns with the circle’s, while the overlay aligns the composite view with the square:

You can achieve layering without an overlay modifier by putting both the modified view and the overlay content into a ZStack. This can produce a simpler view hierarchy, but changes the layout priority that SwiftUI applies to the views. Use the overlay modifier when you want the modified view to dominate the layout.

If you want to specify a ShapeStyle like a Color or a Material as the overlay, use overlay(_:ignoresSafeAreaEdges:) instead. To specify a Shape, use overlay(_:in:fillStyle:).

## See Also

### Layering views

Adding a background to your view

Compose a background behind your view and extend it beyond the safe area insets.

struct ZStack

A view that overlays its subviews, aligning them in both axes.

func zIndex(Double) -> some View

Controls the display order of overlapping views.

func background&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify behind this view.

func background&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to a style.

func background(ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to the default background style.

func background(_:in:fillStyle:)

Sets the view’s background to an insettable shape filled with a style.

func background(in:fillStyle:)

Sets the view’s background to an insettable shape filled with the default background style.

func overlay&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Layers the specified style in front of this view.

func overlay&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Layers a shape that you specify in front of this view.

var backgroundMaterial: Material?

The material underneath the current view.

func containerBackground&lt;S>(S, for: ContainerBackgroundPlacement) -> some View

Sets the container background of the enclosing container using a view.

func containerBackground&lt;V>(for: ContainerBackgroundPlacement, alignment: Alignment, content: () -> V) -> some View

Sets the container background of the enclosing container using a view.

struct ContainerBackgroundPlacement

The placement of a container background.

