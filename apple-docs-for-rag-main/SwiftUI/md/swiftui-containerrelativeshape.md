

- SwiftUI
-  ContainerRelativeShape 

Structure

# ContainerRelativeShape

A shape that is replaced by an inset version of the current container shape. If no container shape was defined, is replaced by a rectangle.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct ContainerRelativeShape
```

## Topics

### Creating the shape

init()

## Relationships

### Conforms To

- Animatable
- BitwiseCopyable
- Copyable
- InsettableShape
- Sendable
- Shape
- View

## See Also

### Setting a container shape

func containerShape&lt;T>(T) -> some View

Sets the container shape to use for any container relative shape within this view.

protocol InsettableShape

A shape type that is able to inset itself to produce another shape.

