

- SceneKit
- SCNNode
-  look(at:up:localFront:) 

Instance Method

# look(at:up:localFront:)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func look(
    at worldTarget: SCNVector3,
    up worldUp: SCNVector3,
    localFront: SCNVector3
)
```

## Parameters 

`worldTarget`  

The point, in world space, to face the node toward.

`worldUp`  

The direction vector, in world space, that should appear as “up” from the rotated node’s point of view.

`localFront`  

The direction vector, in the node’s local space, that should orient toward the target point.

## Discussion

The effects of this method are animatable; that is, calling this method during an implicit-animation transaction animates the rotation effect. (See Animating SceneKit Content.)

## See Also

### Related Documentation

func simdLook(at: simd_float3, up: simd_float3, localFront: simd_float3)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

### Performing Node-Relative Operations (SceneKit Types)

func rotate(by: SCNQuaternion, aroundTarget: SCNVector3)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

func localTranslate(by: SCNVector3)

Changes the node’s position relative to its current position.

func localRotate(by: SCNQuaternion)

Changes the node’s orientation relative to its current orientation.

func look(at: SCNVector3)

Changes the node’s orientation so that its local forward vector points toward the specified location.

