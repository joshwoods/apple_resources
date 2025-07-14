

- SpriteKit
- SKReferenceNode
-  resolve() 

Instance Method

# resolve()

Loads the reference node’s content and adds it as a new child node.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func resolve()
```

**watchOS**

``` source
func resolve()
```

## Discussion

The archive is deserialized and the root node is added as a child of the reference node. If this method is called on a reference node whose content is already loaded, the existing node tree is discarded and replaced with a fresh copy of the archive’s data.

SpriteKit calls this method automatically if the scene renders the reference node and the reference node has not previously been loaded.

