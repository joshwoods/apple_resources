

- SpriteKit
- SKNode
-  init(fileNamed:) 

Initializer

# init(fileNamed:)

Creates a new node by loading an archive file from the game’s main bundle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init?(fileNamed filename: String)
```

**watchOS**

``` source
convenience init?(fileNamed filename: String)
```

## Parameters 

`filename`  

The name of the file, without a file extension. The file must be in the app’s main bundle and have a `.sks` filename extension.

## Return Value

The unarchived node object.

## Mentioned in 

Creating a Scene from a File

## Discussion

If you call this method on a subclass of the SKScene class and the object in the archive is an SKScene object, the returned object is initialized as if it is a member of the subclass. You use this behavior to create scene layouts in the Xcode Editor and provide custom behaviors in your subclass.

## See Also

### First Steps

Getting Started with Nodes

Learn about the fundamental properties that provide a foundation for all other nodes.

init()

Initializes a blank node.

init?(coder: NSCoder)

Called when a node is initialized from an .sks file.

convenience init(fileNamed: String, securelyWithClasses: Set&lt;AnyHashable>) throws

