

- SwiftUI
- Shape
-  role 

Type Property

# role

An indication of how to style a shape.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
static var role: ShapeRole { get }
```

**Required** Default implementation provided.

## Discussion

SwiftUI looks at a shape’s role when deciding how to apply a ShapeStyle at render time. The Shape protocol provides a default implementation with a value of ShapeRole.fill. If you create a composite shape, you can provide an override of this property to return another value, if appropriate.

## Default Implementations

### Shape Implementations

static var role: ShapeRole

An indication of how to style a shape.

