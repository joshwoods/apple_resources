

- SpriteKit
- SKShapeNode
-  init(ellipseIn:) 

Initializer

# init(ellipseIn:)

Creates a shape node with an elliptical path that fills the specified rectangle.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(ellipseIn rect: CGRect)
```

**watchOS**

``` source
convenience init(ellipseIn rect: CGRect)
```

## Parameters 

`rect`  

A rectangle, relative to the node’s origin.

## Return Value

A new shape node.

## See Also

### Creating an Ellipse Shape

convenience init(ellipseOf: CGSize)

Creates a shape node with an elliptical path centered on the node’s origin.

