

- ARKit
- RoomAnchor
-  geometries(of:) 

Instance Method

# geometries(of:)

Returns the disjoint mesh geometries of a given classification.

visionOS 2.0+

``` source
func geometries(of classification: MeshAnchor.MeshClassification) -> [MeshAnchor.Geometry]
```

## Parameters 

`classification`  

The mesh classification to look for.

## Return Value

An array of MeshAnchor.Geometry structures that match the provided classification.

## Discussion

\##Discussion

`RoomAnchor.geometries(of:)` supports the `floor` and `wall` mesh classifications.

## See Also

### Inspecting a room anchor

func contains(SIMD3&lt;Float>) -> Bool

Returns a Boolean value that indicates whether a room contains the provided point.

var description: String

A textual representation of this anchor.

