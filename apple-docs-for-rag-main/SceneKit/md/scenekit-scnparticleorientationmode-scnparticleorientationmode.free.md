

- SceneKit
- SCNParticleOrientationMode
-  SCNParticleOrientationMode.free 

Case

# SCNParticleOrientationMode.free

Particle orientations are not restricted; they may rotate freely in all axes.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case free
```

## Discussion

When using this mode, you can modify the rotation axis of each particle with the rotationAxis key.

## See Also

### Constants

case billboardScreenAligned

Each particle’s orientation is always fixed with respect to the point of view camera.

case billboardViewAligned

Each particle always faces the point of view camera (but may rotate about an axis parallel to the view direction).

case billboardYAligned

The y-axis direction of each particle is always fixed with respect to the point of view camera.

