

- SpriteKit
- SKShapeNode
-  init(rectOf:) 

Initializer

# init(rectOf:)

Creates a shape node with a rectangular path centered on the node’s origin.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
convenience init(rectOf size: CGSize)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(rectOf size: CGSize)
```

## Parameters 

`size`  

The size of the rectangle.

## Return Value

A new shape node.

## See Also

### Creating a Shape from a Rectangle

convenience init(rect: CGRect)

Creates a shape node with a rectangular path.

convenience init(rect: CGRect, cornerRadius: CGFloat)

Creates a shape with a rectangular path that has rounded corners.

convenience init(rectOf: CGSize, cornerRadius: CGFloat)

Creates a shape with a rectangular path that has rounded corners centered on the node’s position.

