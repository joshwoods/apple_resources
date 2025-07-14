

- SceneKit
- SCNNode
-  simdLocalRotate(by:) 

Instance Method

# simdLocalRotate(by:)

Changes the node’s orientation relative to its current orientation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func simdLocalRotate(by rotation: simd_quatf)
```

## Parameters 

`rotation`  

The axis and angle of rotation to apply, in node-local space, expressed as a quaternion.

## Discussion

This method rotates the node according to its simdPivot transform.

The effects of this method are animatable; that is, calling this method during an implicit-animation transaction animates the rotation effect. (See Animating SceneKit Content.)

## See Also

### Related Documentation

func localRotate(by: SCNQuaternion)

Changes the node’s orientation relative to its current orientation.

### Performing Node-Relative Operations

func simdRotate(by: simd_quatf, aroundTarget: simd_float3)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

func simdLocalTranslate(by: simd_float3)

Changes the node’s position relative to its current position.

func simdLook(at: simd_float3)

Changes the node’s orientation so that its local forward vector points toward the specified location.

func simdLook(at: simd_float3, up: simd_float3, localFront: simd_float3)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

