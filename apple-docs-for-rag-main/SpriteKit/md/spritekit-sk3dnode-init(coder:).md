

- SpriteKit
- SK3DNode
-  init(coder:) 

Initializer

# init(coder:)

Tells you when to initialize a 3D node that has been unarchived.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

**watchOS**

``` source
init?(coder aDecoder: NSCoder)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init?(coder aDecoder: NSCoder)
```

## Discussion

Do not call this function directly; it is called by the system when you should initialize a 3D node that has been unarchived.

## See Also

### Creating 3D Nodes

init(viewportSize: CGSize)

Initializes a new 3D node.

