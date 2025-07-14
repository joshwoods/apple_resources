

- SceneKit
- SCNTransformConstraint
-  orientationConstraint(inWorldSpace:with:) 

Type Method

# orientationConstraint(inWorldSpace:with:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class func orientationConstraint(
    inWorldSpace world: Bool,
    with block: @escaping (SCNNode, SCNQuaternion) -> SCNQuaternion
) -> Self
```

