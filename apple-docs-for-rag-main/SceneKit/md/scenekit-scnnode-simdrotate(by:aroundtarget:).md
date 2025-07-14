

- SceneKit
- SCNNode
-  simdRotate(by:aroundTarget:) 

Instance Method

# simdRotate(by:aroundTarget:)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func simdRotate(
    by worldRotation: simd_quatf,
    aroundTarget worldTarget: simd_float3
)
```

## Parameters 

`worldRotation`  

The axis and angle of rotation to apply, in scene space, expressed as a quaternion.

`worldTarget`  

The center point, in scene space, about which to rotate.

## Discussion

The effects of this method are animatable; that is, calling this method during an implicit-animation transaction animates the rotation effect. (See Animating SceneKit Content.)

## See Also

### Related Documentation

func rotate(by: SCNQuaternion, aroundTarget: SCNVector3)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

### Performing Node-Relative Operations

func simdLocalTranslate(by: simd_float3)

Changes the node’s position relative to its current position.

func simdLocalRotate(by: simd_quatf)

Changes the node’s orientation relative to its current orientation.

func simdLook(at: simd_float3)

Changes the node’s orientation so that its local forward vector points toward the specified location.

func simdLook(at: simd_float3, up: simd_float3, localFront: simd_float3)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

