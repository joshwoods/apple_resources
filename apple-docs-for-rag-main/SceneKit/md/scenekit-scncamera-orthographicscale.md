

- SceneKit
- SCNCamera
-  orthographicScale 

Instance Property

# orthographicScale

Specifies the camera’s magnification factor when using an orthographic projection.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var orthographicScale: Double { get set }
```

## Discussion

In an orthographic projection, equally sized objects appear equally sized regardless of their distance from the camera. To switch between orthographic and perspective projections, see the usesOrthographicProjection property.

## See Also

### Managing the Projection Transform

var projectionTransform: SCNMatrix4

The camera’s projection transformation.

var usesOrthographicProjection: Bool

A Boolean value that determines whether the camera uses an orthographic projection.

