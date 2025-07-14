

- SceneKit
- SCNLevelOfDetail
-  worldSpaceDistance 

Instance Property

# worldSpaceDistance

The minimum distance from the current point of view for this level of detail to appear.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var worldSpaceDistance: CGFloat { get }
```

## Discussion

When rendering a geometry with associated levels of detail, SceneKit calculates the distance from the current point of view to the geometry’s parent node, then renders the geometry for the SCNLevelOfDetail object with the largest `distance` parameter less than that distance.

## See Also

### Inspecting a Level of Detail

var geometry: SCNGeometry?

The geometry associated with this level of detail.

var screenSpaceRadius: CGFloat

The maximum radius (in pixels) of the geometry’s bounding sphere for this level of detail to appear.

