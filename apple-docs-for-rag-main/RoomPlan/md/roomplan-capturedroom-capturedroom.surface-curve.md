

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
-  curve 

Instance Property

# curve

An object that represents the curve of a surface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var curve: CapturedRoom.Surface.Curve? { get }
```

## See Also

### Shaping a surface

var completedEdges: Set&lt;CapturedRoom.Surface.Edge>

An array of edges that outline the surface.

enum Edge

An object that represents a single edge of a surface.

struct Curve

An object that represents a single curve of a surface.

var polygonCorners: [simd_float3]

A 2D polygon that represents nonuniform wall heights and floor shapes.

