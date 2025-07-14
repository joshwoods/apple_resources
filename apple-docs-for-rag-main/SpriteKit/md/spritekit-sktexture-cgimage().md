

- SpriteKit
- SKTexture
-  cgImage() 

Instance Method

# cgImage()

Returns the texture’s image data as a Quartz 2D image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cgImage() -> CGImage
```

## Discussion

The cgImage() property returns the contents of a texture as a Quartz Image.

As an example use, you can create an image from a portion of your scene and save it to disk by doing the following:

1.  Use the texture(from:) method to render the scene’s contents to a texture.

2.  Call cgImage() on the result.

3.  Use CGImageDestination to write the `CGImage` out to disk.

