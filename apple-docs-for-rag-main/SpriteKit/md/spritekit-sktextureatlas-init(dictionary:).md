

- SpriteKit
- SKTextureAtlas
-  init(dictionary:) 

Initializer

# init(dictionary:)

Creates a texture atlas from a set of image files.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
convenience init(dictionary properties: [String : Any])
```

## Parameters 

`properties`  

A dictionary that defines which textures are to be merged into the atlas.

## Return Value

A new texture atlas object.

## Mentioned in 

About Texture Atlases

## Discussion

Normally, Xcode creates texture atlases at compile time from the image files included in your project. These atlases are compiled and installed inside the app bundle. However, sometimes the assets needed to create a texture atlas are not available at compile time. For example, those assets might be procedurally generated or downloaded from the network. However, you still want the benefit of texture atlases to reduce the number of state changes required in the hardware. You can use this method to generate an atlas object at runtime. This is a potentially expensive operation best performed when your game loop is not running.

The keys in the dictionary represent the names of the individual textures. The associated object for each key can be:

- An NSString object that contains a file system path to a file that contains the texture

- An NSURL object that contains a file system path to a file that contains the texture

- A UIImage object

- An NSImage object

## See Also

### Creating a Texture Atlas Programmatically

convenience init(named: String)

Creates a texture atlas from data stored in the app bundle.

