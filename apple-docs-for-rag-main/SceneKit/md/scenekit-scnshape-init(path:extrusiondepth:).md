

- SceneKit
- SCNShape
-  init(path:extrusionDepth:) 

Initializer

# init(path:extrusionDepth:)

Creates a shape geometry with the specified path and extrusion depth.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

**macOS**

``` source
convenience init(
    path: NSBezierPath?,
    extrusionDepth: CGFloat
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
convenience init(
    path: UIBezierPath?,
    extrusionDepth: CGFloat
)
```

## Parameters 

`path`  

The two-dimensional path forming the basis of the shape.

`extrusionDepth`  

The thickness of the extruded shape along the z-axis.

## Return Value

A shape geometry.

## Discussion

SceneKit determines the filled area of the path using the even-odd winding rule (see Winding Rules in Cocoa Drawing Guide) and extrudes this area to create a three-dimensional geometry. The result of extruding a self-intersecting path is undefined.

The extruded shape is centered at the zero point of its z-axis. For example, an extrusion depth of `1.0` creates a shape that extends from `-0.5` to `0.5` along the z-axis. An extrusion depth of zero creates a flat, one-sided shape.

The path’s flatness (see flatness in NSBezierPath) determines the level of detail SceneKit uses in building a three-dimensional shape from the path. A larger flatness value results in fewer polygons to render, increasing performance, and a smaller flatness value increases the smoothness of curves at a cost to performance.

