

- SceneKit
- SCNParticleSortingMode
-  SCNParticleSortingMode.none 

Case

# SCNParticleSortingMode.none

Particles are not sorted; they may be rendered in any order.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case none
```

## See Also

### Constants

case projectedDepth

Particles farther from the point of view (as measured using projected depth) are rendered before closer particles.

case distance

Particles farther from the point of view (as measured using distance from the camera in scene space) are rendered before closer particles.

case oldestFirst

Particles emitted earlier are rendered before particles emitted more recently.

case youngestFirst

Particles emitted more recently are rendered before particles emitted earlier.

