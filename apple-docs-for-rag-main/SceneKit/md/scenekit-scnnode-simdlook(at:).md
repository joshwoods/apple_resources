

- SceneKit
- SCNNode
-  simdLook(at:) 

Instance Method

# simdLook(at:)

Changes the node’s orientation so that its local forward vector points toward the specified location.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func simdLook(at worldTarget: simd_float3)
```

## Parameters 

`worldTarget`  

The point, in world space, to face the node toward.

## Discussion

Using this method is equivalent to calling the simdLook(at:up:localFront:) method and passing the node’s simdWorldUp and simdLocalFront vectors for the corresponding parameters.

The effects of this method are animatable; that is, calling this method during an implicit-animation transaction animates the rotation effect. (See Animating SceneKit Content.)

## See Also

### Related Documentation

func look(at: SCNVector3)

Changes the node’s orientation so that its local forward vector points toward the specified location.

### Performing Node-Relative Operations

func simdRotate(by: simd_quatf, aroundTarget: simd_float3)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

func simdLocalTranslate(by: simd_float3)

Changes the node’s position relative to its current position.

func simdLocalRotate(by: simd_quatf)

Changes the node’s orientation relative to its current orientation.

func simdLook(at: simd_float3, up: simd_float3, localFront: simd_float3)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

