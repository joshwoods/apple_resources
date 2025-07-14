

- GameplayKit
- GKPath
-  float3(at:) 

Instance Method

# float3(at:)

Returns the 3D point at the specified index in the path’s list of vertices.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func float3(at index: Int) -> vector_float3
```

## Parameters 

`index`  

The index of the vertex to return, between `0` and the numPoints value.

## Return Value

The vertex at the specified index.

## Discussion

You define a path’s vertices when creating it, either directly with the initWithFloat3Points:count:radius:cyclical: initializer or indirectly with the init(graphNodes:radius:) initializer.

If the path is a 2D path, this method is still functional, but returns 3D vectors whose z-component is always zero.

## See Also

### Inspecting a Path’s Shape

var numPoints: Int

The number of vertices in the path.

func float2(at: Int) -> vector_float2

Returns the 2D point at the specified index in the path’s list of vertices.

func point(at: Int) -> vector_float2

Returns the 2D point at the specified index in the path’s list of vertices.

Deprecated

