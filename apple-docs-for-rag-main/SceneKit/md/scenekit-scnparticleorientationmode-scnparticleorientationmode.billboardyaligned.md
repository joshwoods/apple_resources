

- SceneKit
- SCNParticleOrientationMode
-  SCNParticleOrientationMode.billboardYAligned 

Case

# SCNParticleOrientationMode.billboardYAligned

The y-axis direction of each particle is always fixed with respect to the point of view camera.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case billboardYAligned
```

## Discussion

Use this mode to allow each particle to rotate freely about its y-axis (as determined by the particleAngle and particleAngularVelocity properties or the angle key), but prevent it from rotating around any other axis.

## See Also

### Constants

case billboardScreenAligned

Each particle’s orientation is always fixed with respect to the point of view camera.

case billboardViewAligned

Each particle always faces the point of view camera (but may rotate about an axis parallel to the view direction).

case free

Particle orientations are not restricted; they may rotate freely in all axes.

