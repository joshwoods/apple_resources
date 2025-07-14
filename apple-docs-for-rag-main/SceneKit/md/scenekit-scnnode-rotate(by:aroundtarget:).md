

- SceneKit
- SCNNode
-  rotate(by:aroundTarget:) 

Instance Method

# rotate(by:aroundTarget:)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func rotate(
    by worldRotation: SCNQuaternion,
    aroundTarget worldTarget: SCNVector3
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

func simdRotate(by: simd_quatf, aroundTarget: simd_float3)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

### Performing Node-Relative Operations (SceneKit Types)

func localTranslate(by: SCNVector3)

Changes the node’s position relative to its current position.

func localRotate(by: SCNQuaternion)

Changes the node’s orientation relative to its current orientation.

func look(at: SCNVector3)

Changes the node’s orientation so that its local forward vector points toward the specified location.

func look(at: SCNVector3, up: SCNVector3, localFront: SCNVector3)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

