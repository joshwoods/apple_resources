

- SceneKit
- SCNPhysicsShape
-  transforms 

Instance Property

# transforms

The array of transforms that was used to create a compound shape.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var transforms: [NSValue]? { get }
```

## Discussion

You provide this array of NSValue objects, each containing an SCNMatrix4 value, in the init(shapes:transforms:) method to create a compound shape. Use this array along with the sourceObject property to recover the information that was used to create the shape.

If the shape was created with the init(geometry:options:) or init(node:options:) method, this property’s value is `nil`.

## See Also

### Getting Information About a Shape

var sourceObject: Any

The object that was used to create the shape.

var options: [SCNPhysicsShape.Option : Any]?

The options dictionary that was used to create the shape.

