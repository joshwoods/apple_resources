

- DeviceActivity
- DeviceActivityReport
-  background(in:fillStyle:) 

Instance Method

# background(in:fillStyle:)

Sets the view’s background to an insettable shape filled with the default background style.

DeviceActivitySwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func background(
    in shape: S,
    fillStyle: FillStyle = FillStyle()
) -> some View where S : InsettableShape
```

## Parameters 

`shape`  

An instance of a type that conforms to `InsettableShape` that SwiftUI draws behind the view using the `ShapeStyle/background` shape style.

`fillStyle`  

The `FillStyle` to use when drawing the shape. The default style uses the nonzero winding number rule and antialiasing.

## Return Value

A view with the specified insettable shape drawn behind it.

## Discussion

This modifier behaves like `View/background(_:in:fillStyle:)`, except that it always uses the `ShapeStyle/background` shape style to fill the specified insettable shape. For example, you can use a `RoundedRectangle` as a background on a `Label`:

```
ZStack {
    Color.teal
    Label("Flag", systemImage: "flag.fill")
        .padding()
        .background(in: RoundedRectangle(cornerRadius: 8))
}
```

Without the background modifier, the fill color shows through the label. With the modifier, the label’s text and icon appear backed by a shape filled with a color that’s appropriate for light or dark appearance:

To create a background with other `View` types — or with a stack of views — use `View/background(alignment:content:)` instead. To add a `ShapeStyle` as a background, use `View/background(_:ignoresSafeAreaEdges:)`.

