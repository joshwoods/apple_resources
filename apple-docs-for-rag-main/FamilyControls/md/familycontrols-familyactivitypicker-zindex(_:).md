

- FamilyControls
- FamilyActivityPicker
-  zIndex(\_:) 

Instance Method

# zIndex(\_:)

Controls the display order of overlapping views.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func zIndex(_ value: Double) -> some View
```

## Parameters 

`value`  

A relative front-to-back ordering for this view; the default is `0`.

## Discussion

Use `zIndex(_:)` when you want to control the front-to-back ordering of views.

In this example there are two overlapping rotated rectangles. The frontmost is represented by the larger index value.

```
VStack {
    Rectangle()
        .fill(Color.yellow)
        .frame(width: 100, height: 100, alignment: .center)
        .zIndex(1) // Top layer.

    Rectangle()
        .fill(Color.red)
        .frame(width: 100, height: 100, alignment: .center)
        .rotationEffect(.degrees(45))
        // Here a zIndex of 0 is the default making
        // this the bottom layer.
}
```

## See Also

### Layering

func background&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify behind this view.

func listRowInsets(EdgeInsets?) -> some View

Applies an inset to the rows in a list.

func overlay&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify in front of this view.

