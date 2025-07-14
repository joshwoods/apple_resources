

- SpriteKit
- SKShapeNode
-  init(rectOf:cornerRadius:) 

Initializer

# init(rectOf:cornerRadius:)

Creates a shape with a rectangular path that has rounded corners centered on the node’s position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
convenience init(
    rectOf size: CGSize,
    cornerRadius: CGFloat
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(
    rectOf size: CGSize,
    cornerRadius: CGFloat
)
```

## Parameters 

`size`  

The size of the rectangle.

`cornerRadius`  

The radius of the rounded corners. The radius should not be a negative number. The value should be no larger than half of the rectangle’s width or height, whichever is smaller.

## Return Value

A new shape node.

## See Also

### Creating a Shape from a Rectangle

convenience init(rect: CGRect)

Creates a shape node with a rectangular path.

convenience init(rectOf: CGSize)

Creates a shape node with a rectangular path centered on the node’s origin.

convenience init(rect: CGRect, cornerRadius: CGFloat)

Creates a shape with a rectangular path that has rounded corners.

