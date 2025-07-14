

- GameplayKit
- GKPath
-  point(at:) Deprecated

Instance Method

# point(at:)

Returns the 2D point at the specified index in the path’s list of vertices.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func point(at index: Int) -> vector_float2
```

Deprecated

Use the float2(at:) method instead.

## Parameters 

`index`  

The index of the vertex to return, between `0` and the numPoints value.

## Return Value

The vertex at the specified index.

## See Also

### Inspecting a Path’s Shape

var numPoints: Int

The number of vertices in the path.

func float2(at: Int) -> vector_float2

Returns the 2D point at the specified index in the path’s list of vertices.

func float3(at: Int) -> vector_float3

Returns the 3D point at the specified index in the path’s list of vertices.

