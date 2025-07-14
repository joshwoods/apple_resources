

- SceneKit
- SCNMorpherCalculationMode
-  SCNMorpherCalculationMode.additive 

Case

# SCNMorpherCalculationMode.additive

Target weights may take on any value, and weighted contributions for each target are added to the base geometry,

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case additive
```

## See Also

### Constants

case normalized

Target weights must be in the range between `0.0` and `1.0`, and the contribution of the base geometry to the morphed surface is related to the sum of target weights. This is the default mode.

