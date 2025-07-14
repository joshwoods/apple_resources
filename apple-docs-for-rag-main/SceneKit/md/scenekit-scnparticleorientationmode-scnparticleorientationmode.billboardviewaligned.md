

- SceneKit
- SCNParticleOrientationMode
-  SCNParticleOrientationMode.billboardViewAligned 

Case

# SCNParticleOrientationMode.billboardViewAligned

Each particle always faces the point of view camera (but may rotate about an axis parallel to the view direction).

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case billboardViewAligned
```

## Discussion

Use this mode for particle images whose individual appearance depends on a location and orientation in scene space, such as “impostor” images representing trees or clouds in a scene.

## See Also

### Constants

case billboardScreenAligned

Each particle’s orientation is always fixed with respect to the point of view camera.

case free

Particle orientations are not restricted; they may rotate freely in all axes.

case billboardYAligned

The y-axis direction of each particle is always fixed with respect to the point of view camera.

