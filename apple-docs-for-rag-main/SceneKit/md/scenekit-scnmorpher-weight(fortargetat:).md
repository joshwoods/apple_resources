

- SceneKit
- SCNMorpher
-  weight(forTargetAt:) 

Instance Method

# weight(forTargetAt:)

Returns the weight value for the specified target index.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
func weight(forTargetAt targetIndex: Int) -> CGFloat
```

## Parameters 

`targetIndex`  

The index of a geometry in the morpher’s targets array.

## Return Value

A number indicating the contribution of the target geometry to the blended surface, generally between `0.0` and `1.0`.

## Discussion

Target geometries and their weights determine the current form of the surface produced by the morpher. For example, if a morpher has one target whose weight is `0.5`, the form of the resulting surface will be halfway between those of the base geometry and the target geometry.

## See Also

### Blending between Morph Targets

func setWeight(CGFloat, forTargetAt: Int)

Specifies a weight value at a specified target index.

