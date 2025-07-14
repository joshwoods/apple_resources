

- SceneKit
- SCNParticleSortingMode
-  SCNParticleSortingMode.projectedDepth 

Case

# SCNParticleSortingMode.projectedDepth

Particles farther from the point of view (as measured using projected depth) are rendered before closer particles.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case projectedDepth
```

## Discussion

Typically you use this sorting mode in conjunction with the SCNParticleOrientationMode.billboardScreenAligned orientation mode.

## See Also

### Constants

case none

Particles are not sorted; they may be rendered in any order.

case distance

Particles farther from the point of view (as measured using distance from the camera in scene space) are rendered before closer particles.

case oldestFirst

Particles emitted earlier are rendered before particles emitted more recently.

case youngestFirst

Particles emitted more recently are rendered before particles emitted earlier.

