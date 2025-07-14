

- SpriteKit
- SKSpriteNode
-  init(color:size:) 

Initializer

# init(color:size:)

Initializes a single-color sprite node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**macOS**

``` source
@MainActor
convenience init(
    color: NSColor,
    size: CGSize
)
```

**watchOS**

``` source
convenience init(
    color: UIColor,
    size: CGSize
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
convenience init(
    color: UIColor,
    size: CGSize
)
```

## Parameters 

`color`  

The color for the resulting sprite node.

`size`  

The size of the sprite node in points.

## Return Value

A newly initialized sprite node.

## Discussion

Although textured nodes are the most common way to use the SKSpriteNode class, you can also create sprite nodes without a texture. The behavior of the class changes when the node lacks a texture:

- The sprite node that is returned from this method has its texture property set to `nil`.

- There is no texture to stretch, so the centerRect parameter is ignored.

- There is no colorization step; the color property is used as the sprite’s color.

- The sprite node’s alpha component is used to determine how it is blended into the buffer.

Listing 1 shows how to create a red sprite node `100 x 100` points in size.

Listing 1. Creating a non-textured sprite node

```
let node = SKSpriteNode(color: .red,
                        size: CGSize(width: 100, height: 100))
```

