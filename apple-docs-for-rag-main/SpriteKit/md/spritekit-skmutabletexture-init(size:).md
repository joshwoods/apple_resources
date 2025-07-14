

- SpriteKit
- SKMutableTexture
-  init(size:) 

Initializer

# init(size:)

Initializes an empty texture with a specific size.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(size: CGSize)
```

## Parameters 

`size`  

The size of the texture, in pixels.

## Return Value

An empty mutable texture.

## Discussion

You must call the modifyPixelData(_:) method at least once before using this texture.

## See Also

### Creating an Empty Mutable Texture

init(size: CGSize, pixelFormat: Int32)

Initializes an empty texture with a specific size and format.

