

- SceneKit
- SCNParticleInputMode
-  SCNParticleInputMode.overOtherProperty 

Case

# SCNParticleInputMode.overOtherProperty

The controller’s effect on a particle property is a function of another of the particle’s properties.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case overOtherProperty
```

## Discussion

Use the inputProperty property to specify the input property, and the inputBias and inputScale properties to refine the relationship between a range of property values into a range of input values for the controller’s animation.

## See Also

### Constants

case overLife

The controller’s effect on a particle property is a function of the time since the particle’s birth.

case overDistance

The controller’s effect on a particle property is a function of the particle’s distance from the position of a specified node.

