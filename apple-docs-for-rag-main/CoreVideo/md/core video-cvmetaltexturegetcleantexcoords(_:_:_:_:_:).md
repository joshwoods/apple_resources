

- Core Video
-  CVMetalTextureGetCleanTexCoords(\_:\_:\_:\_:\_:) 

Function

# CVMetalTextureGetCleanTexCoords(\_:\_:\_:\_:\_:)

Returns convenient normalized texture coordinates for the part of the image that should be displayed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func CVMetalTextureGetCleanTexCoords(
    _ image: CVMetalTexture,
    _ lowerLeft: UnsafeMutablePointer,
    _ lowerRight: UnsafeMutablePointer,
    _ upperRight: UnsafeMutablePointer,
    _ upperLeft: UnsafeMutablePointer
)
```

## Parameters 

`image`  

A CoreVideo Metal texture-based image buffer.

## Discussion

This function automatically takes into account whether or not the texture is flipped.

## See Also

### Inspecting Textures

func CVMetalTextureGetTexture(CVMetalTexture) -> (any MTLTexture)?

Returns the Metal texture object for the image buffer.

func CVMetalTextureIsFlipped(CVMetalTexture) -> Bool

Returns a Boolean value indicating whether the texture image is vertically flipped.

func CVMetalTextureGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a CoreVideo Metal texture-based image buffer.

