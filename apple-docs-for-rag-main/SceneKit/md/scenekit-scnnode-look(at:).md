

- SceneKit
- SCNNode
-  look(at:) 

Instance Method

# look(at:)

Changes the node’s orientation so that its local forward vector points toward the specified location.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func look(at worldTarget: SCNVector3)
```

## Parameters 

`worldTarget`  

The point, in world space, to face the node toward.

## Discussion

Using this method is equivalent to calling the look(at:up:localFront:) method and passing the node’s worldUp and localFront vectors for the corresponding parameters.

The effects of this method are animatable; that is, calling this method during an implicit-animation transaction animates the rotation effect. (See Animating SceneKit Content.)

## See Also

### Related Documentation

func simdLook(at: simd_float3)

Changes the node’s orientation so that its local forward vector points toward the specified location.

### Performing Node-Relative Operations (SceneKit Types)

func rotate(by: SCNQuaternion, aroundTarget: SCNVector3)

Changes the node’s position and orientation, relative to its current transform, through a rotation around the specified point in scene space.

func localTranslate(by: SCNVector3)

Changes the node’s position relative to its current position.

func localRotate(by: SCNQuaternion)

Changes the node’s orientation relative to its current orientation.

func look(at: SCNVector3, up: SCNVector3, localFront: SCNVector3)

Changes the node’s orientation so that the specified forward vector points toward the specified location.

