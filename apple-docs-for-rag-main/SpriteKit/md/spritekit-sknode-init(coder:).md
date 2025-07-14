

- SpriteKit
- SKNode
-  init(coder:) 

Initializer

# init(coder:)

Called when a node is initialized from an .sks file.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init?(coder aDecoder: NSCoder)
```

**watchOS**

``` source
init?(coder aDecoder: NSCoder)
```

## See Also

### First Steps

Getting Started with Nodes

Learn about the fundamental properties that provide a foundation for all other nodes.

init()

Initializes a blank node.

convenience init?(fileNamed: String)

Creates a new node by loading an archive file from the game’s main bundle.

convenience init(fileNamed: String, securelyWithClasses: Set&lt;AnyHashable>) throws

