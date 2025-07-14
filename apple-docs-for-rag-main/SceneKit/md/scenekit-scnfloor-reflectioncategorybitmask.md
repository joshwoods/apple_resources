

- SceneKit
- SCNFloor
-  reflectionCategoryBitMask 

Instance Property

# reflectionCategoryBitMask

A mask that defines which categories of other objects show reflections on the floor.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var reflectionCategoryBitMask: Int { get set }
```

## Discussion

## See Also

### Adding Reflections to a Floor

var reflectivity: CGFloat

The intensity of the scene’s reflection on the floor. Animatable.

var reflectionFalloffEnd: CGFloat

The distance from the floor at which scene contents are no longer reflected. Animatable.

var reflectionFalloffStart: CGFloat

The distance from the floor at which scene contents are reflected at full intensity. Animatable.

var reflectionResolutionScaleFactor: CGFloat

The resolution scale factor of the offscreen buffer that SceneKit uses to render reflections.

