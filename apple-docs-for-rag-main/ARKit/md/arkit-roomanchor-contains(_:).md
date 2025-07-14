

- ARKit
- RoomAnchor
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether a room contains the provided point.

visionOS 2.0+

``` source
func contains(_ point: SIMD3) -> Bool
```

## Parameters 

`point`  

The point to search for.

## Return Value

Returns `true` if the room contains the point, otherwise `false`.

## See Also

### Inspecting a room anchor

func geometries(of: MeshAnchor.MeshClassification) -> [MeshAnchor.Geometry]

Returns the disjoint mesh geometries of a given classification.

var description: String

A textual representation of this anchor.

