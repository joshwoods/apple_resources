

- Core Video
-  CVMetalTextureIsFlipped(\_:) 

Function

# CVMetalTextureIsFlipped(\_:)

Returns a Boolean value indicating whether the texture image is vertically flipped.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func CVMetalTextureIsFlipped(_ image: CVMetalTexture) -> Bool
```

## Parameters 

`image`  

A CoreVideo Metal texture-based image buffer.

## Return Value

If `True`, the texture coordinate `{0,0}` represents the upper left of the texture; if `False`, the texture coordinate `{0,0}` represents the lower left of the texture.

## See Also

### Inspecting Textures

func CVMetalTextureGetTexture(CVMetalTexture) -> (any MTLTexture)?

Returns the Metal texture object for the image buffer.

func CVMetalTextureGetCleanTexCoords(CVMetalTexture, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

Returns convenient normalized texture coordinates for the part of the image that should be displayed.

func CVMetalTextureGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a CoreVideo Metal texture-based image buffer.

