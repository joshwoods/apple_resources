

- SceneKit
- SCNNode
-  simdLocalTranslate(by:) 

Instance Method

# simdLocalTranslate(by:)

Changes the node’s position relative to its current position.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func simdLocalTranslate(by translation: simd_float3)
```

## Parameters 

`translation`  

The distance, in node-local space, by which to move the node.

## Discussion

The effects of this method are animatable; that is, calling this method during an implicit-animation transaction animates the move. (See Animating SceneKit Content.)

## See Also

### Related Documentation

func localTranslate(by: SCNVector3)

Changes the node’s position relative to its current position.

### Performing Node-Relative Operations

func simdRotate(by: simd_quatf, aroundTarget: simd_float3)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

func simdLocalRotate(by: simd_quatf)

Changes the node’s orientation relative to its current orientation.

func simdLook(at: simd_float3)

Changes the node’s orientation so that its local forward vector points toward the specified location.

func simdLook(at: simd_float3, up: simd_float3, localFront: simd_float3)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

