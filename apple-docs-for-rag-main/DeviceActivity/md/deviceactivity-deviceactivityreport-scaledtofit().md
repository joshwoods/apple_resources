

- DeviceActivity
- DeviceActivityReport
-  scaledToFit() 

Instance Method

# scaledToFit()

Scales this view to fit its parent.

DeviceActivitySwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func scaledToFit() -> some View
```

## Return Value

A view that scales this view to fit its parent, maintaining this view’s aspect ratio.

## Discussion

Use `scaledToFit()` to scale this view to fit its parent, while maintaining the view’s aspect ratio as the view scales.

```
Circle()
    .fill(Color.pink)
    .scaledToFit()
    .frame(width: 300, height: 150)
    .border(Color(white: 0.75))
```

This method is equivalent to calling `View/aspectRatio(_:contentMode:)` with a `nil` aspectRatio and a content mode of `ContentMode/fit`.

