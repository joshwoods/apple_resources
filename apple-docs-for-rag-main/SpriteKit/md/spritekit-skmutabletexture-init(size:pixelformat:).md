

- SpriteKit
- SKMutableTexture
-  init(size:pixelFormat:) 

Initializer

# init(size:pixelFormat:)

Initializes an empty texture with a specific size and format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(
    size: CGSize,
    pixelFormat format: Int32
)
```

## Parameters 

`size`  

The size of the texture, in pixels.

`format`  

A Core Video format code. Three codes are supported: kCVPixelFormatType_32RGBA, kCVPixelFormatType_64RGBAHalf, and kCVPixelFormatType_128RGBAFloat for byte, half-float, and float components respectively.

## Return Value

An empty mutable texture.

## Discussion

You must call the modifyPixelData(_:) method at least once before using this texture.

## See Also

### Creating an Empty Mutable Texture

init(size: CGSize)

Initializes an empty texture with a specific size.

