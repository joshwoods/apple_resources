

- SceneKit
- SCNParticleInputMode
-  SCNParticleInputMode.overDistance 

Case

# SCNParticleInputMode.overDistance

The controller’s effect on a particle property is a function of the particle’s distance from the position of a specified node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case overDistance
```

## Discussion

Use the inputOrigin property to specify the node to measure distance from, and the inputBias and inputScale properties to refine the relationship between a range of distances into a range of input values for the controller’s animation.

## See Also

### Constants

case overLife

The controller’s effect on a particle property is a function of the time since the particle’s birth.

case overOtherProperty

The controller’s effect on a particle property is a function of another of the particle’s properties.

