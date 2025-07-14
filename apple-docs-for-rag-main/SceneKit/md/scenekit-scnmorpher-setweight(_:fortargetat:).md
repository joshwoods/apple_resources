

- SceneKit
- SCNMorpher
-  setWeight(\_:forTargetAt:) 

Instance Method

# setWeight(\_:forTargetAt:)

Specifies a weight value at a specified target index.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
func setWeight(
    _ weight: CGFloat,
    forTargetAt targetIndex: Int
)
```

## Parameters 

`weight`  

A number specifying the contribution of the target geometry to the blended surface, generally between `0.0` and `1.0`.

`targetIndex`  

The index of a geometry in the morpher’s targets array.

## Discussion

Target geometries and their weights determine the current form of the surface produced by the morpher. For example, if a morpher has one target whose weight is `0.5`, the form of the resulting surface will be halfway between those of the base geometry and the target geometry.

You can also animate weights implicitly or explicitly using the keypath `weights[index]`, where `index` corresponds to the `targetIndex` parameter of this method.

## See Also

### Blending between Morph Targets

func weight(forTargetAt: Int) -> CGFloat

Returns the weight value for the specified target index.

