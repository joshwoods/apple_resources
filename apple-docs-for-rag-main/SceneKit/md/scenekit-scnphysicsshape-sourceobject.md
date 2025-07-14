

- SceneKit
- SCNPhysicsShape
-  sourceObject 

Instance Property

# sourceObject

The object that was used to create the shape.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var sourceObject: Any { get }
```

## Discussion

This property, along with the transforms and options properties, provides the information that was used to create the shape. You can use this information, for example, to draw editing or debugging UI in your scene.

- If the shape was created with the init(geometry:options:) method, the source object is an SCNGeometry object, and the options property contains the options affecting the shape’s construction from that geometry.

- If the shape was created with the init(node:options:) method, the source object is an SCNNode object, and the options property contains the options affecting the shape’s construction from that node.

- If the shape was created with the init(shapes:transforms:) method, the source object is an array of SCNPhysicsShape objects and the transforms property describes how those shapes combine to form a compound shape.

## See Also

### Getting Information About a Shape

var options: [SCNPhysicsShape.Option : Any]?

The options dictionary that was used to create the shape.

var transforms: [NSValue]?

The array of transforms that was used to create a compound shape.

