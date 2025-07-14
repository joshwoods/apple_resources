

- Model I/O
- MDLTexture
-  init(named:bundle:) 

Initializer

# init(named:bundle:)

Loads the texture with the specified filename from the specified bundle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init?(
    named name: String,
    bundle bundleOrNil: Bundle?
)
```

## Parameters 

`name`  

The name, including extension, of the image file to load as a texture.

`bundleOrNil`  

The bundle the image file is located in, or `nil` to use the main bundle.

## Return Value

A new texture object for the specified image file, or `nil` if no such file exists.

## Discussion

Calling this method immediately loads image data from the specified file. To instead create a texture object referencing a file and defer loading image data, use the MDLURLTexture class.

This method does not cache the texture objects it creates; calling this method again with the same `name` parameter as a previous call will load image data from the file again.

## See Also

### Loading Textures from a Bundle

convenience init?(named: String)

Loads the texture with the specified filename from the app’s main bundle.

convenience init?(cubeWithImagesNamed: [String])

Loads a cube texture from the specified image files in the app’s main bundle.

convenience init?(cubeWithImagesNamed: [String], bundle: Bundle?)

Loads a cube texture from the specified image files in the specified bundle.

