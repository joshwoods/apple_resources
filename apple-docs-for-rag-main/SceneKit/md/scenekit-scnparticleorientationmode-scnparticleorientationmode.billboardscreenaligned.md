

- SceneKit
- SCNParticleOrientationMode
-  SCNParticleOrientationMode.billboardScreenAligned 

Case

# SCNParticleOrientationMode.billboardScreenAligned

Each particle’s orientation is always fixed with respect to the point of view camera.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case billboardScreenAligned
```

## Discussion

Use this mode for simple particle images whose individual appearance has no relation to scene space, such as spheres, circles, and “œsparkle” artwork.

## See Also

### Constants

case billboardViewAligned

Each particle always faces the point of view camera (but may rotate about an axis parallel to the view direction).

case free

Particle orientations are not restricted; they may rotate freely in all axes.

case billboardYAligned

The y-axis direction of each particle is always fixed with respect to the point of view camera.

