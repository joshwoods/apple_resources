

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
-  polygonCorners 

Instance Property

# polygonCorners

A 2D polygon that represents nonuniform wall heights and floor shapes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var polygonCorners: [simd_float3] { get }
```

## Discussion

This property’s triplet type describes the polygon in local plane coordinates.

## See Also

### Shaping a surface

var completedEdges: Set&lt;CapturedRoom.Surface.Edge>

An array of edges that outline the surface.

enum Edge

An object that represents a single edge of a surface.

var curve: CapturedRoom.Surface.Curve?

An object that represents the curve of a surface.

struct Curve

An object that represents a single curve of a surface.

