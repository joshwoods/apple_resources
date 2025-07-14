

- SceneKit
- SCNShape
-  path 

Instance Property

# path

The two-dimensional path forming the basis of the shape.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

**macOS**

``` source
@NSCopying
var path: NSBezierPath? { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
@NSCopying
var path: UIBezierPath? { get set }
```

## Discussion

SceneKit determines the filled area of the path using the even-odd winding rule (see Winding Rules in Cocoa Drawing Guide) and extrudes this area to create a three-dimensional geometry. The result of extruding a self-intersecting path is undefined.

The path’s flatness (see flatness in NSBezierPath) determines the level of detail SceneKit uses in building a three-dimensional shape from the path—a larger flatness value results in fewer polygons to render, increasing performance.

## See Also

### Modifying a Shape

var extrusionDepth: CGFloat

The thickness of the extruded shape along the z-axis. Animatable.

