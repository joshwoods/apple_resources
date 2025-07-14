

- SpriteKit
- SKShapeNode
-  init(ellipseOf:) 

Initializer

# init(ellipseOf:)

Creates a shape node with an elliptical path centered on the node’s origin.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(ellipseOf size: CGSize)
```

**watchOS**

``` source
convenience init(ellipseOf size: CGSize)
```

## Parameters 

`size`  

The height and width of the ellipse.

## Return Value

A new shape node.

## See Also

### Creating an Ellipse Shape

convenience init(ellipseIn: CGRect)

Creates a shape node with an elliptical path that fills the specified rectangle.

