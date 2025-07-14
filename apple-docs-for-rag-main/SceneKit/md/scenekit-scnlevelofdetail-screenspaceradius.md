

- SceneKit
- SCNLevelOfDetail
-  screenSpaceRadius 

Instance Property

# screenSpaceRadius

The maximum radius (in pixels) of the geometry’s bounding sphere for this level of detail to appear.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var screenSpaceRadius: CGFloat { get }
```

## Discussion

When rendering a geometry with associated levels of detail, SceneKit calculates the radius in pixels of the circle covered by a geometry’s bounding sphere, then renders the geometry for the SCNLevelOfDetail object with the smallest `radius` parameter larger than that circle.

## See Also

### Inspecting a Level of Detail

var geometry: SCNGeometry?

The geometry associated with this level of detail.

var worldSpaceDistance: CGFloat

The minimum distance from the current point of view for this level of detail to appear.

