

- Core Video
-  CVMetalTextureGetTexture(\_:) 

Function

# CVMetalTextureGetTexture(\_:)

Returns the Metal texture object for the image buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func CVMetalTextureGetTexture(_ image: CVMetalTexture) -> (any MTLTexture)?
```

## Parameters 

`image`  

A CoreVideo Metal texture-based image buffer.

## Return Value

The MTLTexture object corresponding to the image buffer.

## See Also

### Inspecting Textures

func CVMetalTextureGetCleanTexCoords(CVMetalTexture, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

Returns convenient normalized texture coordinates for the part of the image that should be displayed.

func CVMetalTextureIsFlipped(CVMetalTexture) -> Bool

Returns a Boolean value indicating whether the texture image is vertically flipped.

func CVMetalTextureGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier for a CoreVideo Metal texture-based image buffer.

