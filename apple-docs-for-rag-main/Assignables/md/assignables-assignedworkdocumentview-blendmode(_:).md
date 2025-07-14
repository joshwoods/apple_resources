

- Assignables
- AssignedWorkDocumentView
-  blendMode(\_:) 

Instance Method

# blendMode(\_:)

Sets the blend mode for compositing this view with overlapping views.

AssignablesSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func blendMode(_ blendMode: BlendMode) -> some View
```

## Parameters 

`blendMode`  

The `BlendMode` for compositing this view.

## Return Value

A view that applies `blendMode` to this view.

## Discussion

Use `blendMode(_:)` to combine overlapping views and use a different visual effect to produce the result. The `BlendMode` enumeration defines many possible effects.

In the example below, the two overlapping rectangles have a `BlendMode/colorBurn` effect applied, which effectively removes the non-overlapping portion of the second image:

```
HStack {
    Color.yellow.frame(width: 50, height: 50, alignment: .center)

    Color.red.frame(width: 50, height: 50, alignment: .center)
        .rotationEffect(.degrees(45))
        .padding(-20)
        .blendMode(.colorBurn)
}
```

