

- SceneKit
- SCNNode
-  localRotate(by:) 

Instance Method

# localRotate(by:)

Changes the node’s orientation relative to its current orientation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func localRotate(by rotation: SCNQuaternion)
```

## Parameters 

`rotation`  

The axis and angle of rotation to apply, in node-local space, expressed as a quaternion.

## Discussion

This method rotates the node according to its pivot transform.

The effects of this method are animatable; that is, calling this method during an implicit-animation transaction animates the rotation effect. (See Animating SceneKit Content.)

## See Also

### Related Documentation

func simdLocalRotate(by: simd_quatf)

Changes the node’s orientation relative to its current orientation.

### Performing Node-Relative Operations (SceneKit Types)

func rotate(by: SCNQuaternion, aroundTarget: SCNVector3)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

func localTranslate(by: SCNVector3)

Changes the node’s position relative to its current position.

func look(at: SCNVector3)

Changes the node’s orientation so that its local forward vector points toward the specified location.

func look(at: SCNVector3, up: SCNVector3, localFront: SCNVector3)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

