

- SceneKit
- SCNParticleBirthLocation
-  SCNParticleBirthLocation.volume 

Case

# SCNParticleBirthLocation.volume

New particles can be created at any location within the volume of the emitter shape.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case volume
```

## Discussion

This value applies only when the emitterShape property specifies one of SceneKit’s built-in basic geometries (SCNPlane, SCNBox, SCNSphere, SCNPyramid, SCNCone, SCNCylinder, SCNCapsule, SCNTube, and SCNTorus).

## See Also

### Constants

case surface

New particles can be created at any location on the surface of the emitter shape.

case vertex

New particles can be created at only at the locations of the vertices in the emitter shape.

