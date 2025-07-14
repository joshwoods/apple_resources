

- GameplayKit
- GKPath
-  numPoints 

Instance Property

# numPoints

The number of vertices in the path.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var numPoints: Int { get }
```

## Discussion

You define a path’s vertices when creating it, either directly with the initWithPoints:count:radius:cyclical: initializer or indirectly with the init(graphNodes:radius:) initializer.

## See Also

### Inspecting a Path’s Shape

func float2(at: Int) -> vector_float2

Returns the 2D point at the specified index in the path’s list of vertices.

func float3(at: Int) -> vector_float3

Returns the 3D point at the specified index in the path’s list of vertices.

func point(at: Int) -> vector_float2

Returns the 2D point at the specified index in the path’s list of vertices.

Deprecated

