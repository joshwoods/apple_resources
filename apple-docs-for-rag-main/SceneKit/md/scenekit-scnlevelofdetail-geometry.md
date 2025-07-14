

- SceneKit
- SCNLevelOfDetail
-  geometry 

Instance Property

# geometry

The geometry associated with this level of detail.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var geometry: SCNGeometry? { get }
```

## Discussion

SceneKit renders this geometry instead of the original geometry when the level of detail is appropriate. Generally, levels of detail with larger worldSpaceDistance values or smaller screenSpaceRadius values should contain less complex geometries.

If the value of this property is `nil`, SceneKit renders no geometry at this level of detail.

## See Also

### Inspecting a Level of Detail

var screenSpaceRadius: CGFloat

The maximum radius (in pixels) of the geometry’s bounding sphere for this level of detail to appear.

var worldSpaceDistance: CGFloat

The minimum distance from the current point of view for this level of detail to appear.

