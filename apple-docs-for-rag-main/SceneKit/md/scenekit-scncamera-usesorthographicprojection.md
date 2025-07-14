

- SceneKit
- SCNCamera
-  usesOrthographicProjection 

Instance Property

# usesOrthographicProjection

A Boolean value that determines whether the camera uses an orthographic projection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var usesOrthographicProjection: Bool { get set }
```

## Discussion

The default value of this property is false, specifying a perspective projection. In a perspective projection, equally sized objects nearer to the camera appear larger than those farther away.

Set the value of this property to true to specify an orthographic projection. In an orthographic projection, equally sized objects appear equally sized regardless of distance from the camera.

To control the magnification factor of an orthographic camera, use its orthographicScale property.

## See Also

### Managing the Projection Transform

var projectionTransform: SCNMatrix4

The camera’s projection transformation.

var orthographicScale: Double

Specifies the camera’s magnification factor when using an orthographic projection.

