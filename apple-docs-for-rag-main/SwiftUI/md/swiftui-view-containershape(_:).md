

- SwiftUI
- View
-  containerShape(\_:) 

Instance Method

# containerShape(\_:)

Sets the container shape to use for any container relative shape within this view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func containerShape(_ shape: T) -> some View where T : InsettableShape
```

## Discussion

The example below defines a view that shows its content with a rounded rectangle background and the same container shape. Any ContainerRelativeShape within the `content` matches the rounded rectangle shape from this container inset as appropriate.

```
struct PlatterContainer : View {
    @ViewBuilder var content: Content
    var body: some View {
        content
            .padding()
            .containerShape(shape)
            .background(shape.fill(.background))
    }
    var shape: RoundedRectangle { RoundedRectangle(cornerRadius: 20) }
}
```

## See Also

### Setting a container shape

protocol InsettableShape

A shape type that is able to inset itself to produce another shape.

struct ContainerRelativeShape

A shape that is replaced by an inset version of the current container shape. If no container shape was defined, is replaced by a rectangle.

