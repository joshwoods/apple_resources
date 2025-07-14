

- SpriteKit
- SKShapeNode
-  init(rect:) 

Initializer

# init(rect:)

Creates a shape node with a rectangular path.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(rect: CGRect)
```

**watchOS**

``` source
convenience init(rect: CGRect)
```

## Parameters 

`rect`  

A rectangle, relative to the node’s origin.

## Return Value

A new shape node.

## See Also

### Creating a Shape from a Rectangle

convenience init(rectOf: CGSize)

Creates a shape node with a rectangular path centered on the node’s origin.

convenience init(rect: CGRect, cornerRadius: CGFloat)

Creates a shape with a rectangular path that has rounded corners.

convenience init(rectOf: CGSize, cornerRadius: CGFloat)

Creates a shape with a rectangular path that has rounded corners centered on the node’s position.

