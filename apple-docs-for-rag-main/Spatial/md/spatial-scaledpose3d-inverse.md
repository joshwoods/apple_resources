

- Spatial
- ScaledPose3D
-  inverse 

Instance Property

# inverse

The scaled pose’s inverse.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
var inverse: ScaledPose3D { get }
```

## See Also

### Inspecting a 3D scaled pose’s properties

var matrix: simd_double4x4

The scaled pose’s underlying matrix.

var position: Point3D

The scaled pose’s position.

var rotation: Rotation3D

The scaled pose’s rotation.

var scale: Double

The scaled pose’s scale.

var customMirror: Mirror

A mirror that reflects the notification.

static var identity: ScaledPose3D

The identity scaled pose.

