

- SpriteKit
- SKNode
-  init(fileNamed:securelyWithClasses:) 

Initializer

# init(fileNamed:securelyWithClasses:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

**watchOS**

``` source
convenience init(
    fileNamed filename: String,
    securelyWithClasses classes: Set
) throws
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(
    fileNamed filename: String,
    securelyWithClasses classes: Set
) throws
```

## See Also

### First Steps

Getting Started with Nodes

Learn about the fundamental properties that provide a foundation for all other nodes.

init()

Initializes a blank node.

convenience init?(fileNamed: String)

Creates a new node by loading an archive file from the game’s main bundle.

init?(coder: NSCoder)

Called when a node is initialized from an .sks file.

