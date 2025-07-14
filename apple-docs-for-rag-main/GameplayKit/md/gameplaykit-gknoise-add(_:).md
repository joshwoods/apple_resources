

- GameplayKit
- GKNoise
-  add(\_:) 

Instance Method

# add(\_:)

Replaces values in the noise field by adding them to values from the specified noise object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func add(_ noise: GKNoise)
```

## Parameters 

`noise`  

The noise object from which to add noise values.

## Discussion

Note that adding noise values can result in values outside the \[-1.0, 1.0\] range used for colorizing noise. If you plan to procduce colorized textures from the noise object, use the remapValues(toCurveWithControlPoints:) method to return results to that range first.

## See Also

### Applying Operations that Combine Noise

func multiply(GKNoise)

Replaces values in the noise field by multiplying them with values from the specified noise object.

func raiseToPower(GKNoise)

Replaces values in the noise field by exponentiating them with values from the specified noise object.

func maximum(GKNoise)

Replaces values in the noise field by choosing the lesser of each value and a corresponding value in the specified noise object.

func minimum(GKNoise)

Replaces values in the noise field by choosing the lesser of each value and a corresponding value in the specified noise object.

