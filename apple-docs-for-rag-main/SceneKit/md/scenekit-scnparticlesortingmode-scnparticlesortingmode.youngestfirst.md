

- SceneKit
- SCNParticleSortingMode
-  SCNParticleSortingMode.youngestFirst 

Case

# SCNParticleSortingMode.youngestFirst

Particles emitted more recently are rendered before particles emitted earlier.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case youngestFirst
```

## See Also

### Constants

case none

Particles are not sorted; they may be rendered in any order.

case projectedDepth

Particles farther from the point of view (as measured using projected depth) are rendered before closer particles.

case distance

Particles farther from the point of view (as measured using distance from the camera in scene space) are rendered before closer particles.

case oldestFirst

Particles emitted earlier are rendered before particles emitted more recently.

