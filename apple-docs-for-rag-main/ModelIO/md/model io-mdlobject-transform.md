

- Model I/O
- MDLObject
-  transform 

Instance Property

# transform

A component that manages this object’s spatial transform and its changes over time.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var transform: (any MDLTransformComponent)? { get set }
```

## Discussion

A transform defines the local coordinate space for an object’s content—that is, its position, orientation, shear, and scale—relative to the coordinate space of the object’s parent. The MDLTransformComponent protocol defines a general interface for objects that manage transforms, including time-based transform information for assets that include animation data. By default, Model I/O uses the MDLTransform object for this property; however, you can also use a custom class that adopts the MDLTransformComponent protocol to support alternative ways of calculating or storing transform data.

Note

Reading or writing this property is equivalent to calling the componentConforming(to:) or setComponent(_:for:) method with the MDLTransformComponent protocol.

## See Also

### Working with Objects in Space

func boundingBox(atTime: TimeInterval) -> MDLAxisAlignedBoundingBox

Returns the minimum region entirely enclosing the object’s contents at the specified time sample.

