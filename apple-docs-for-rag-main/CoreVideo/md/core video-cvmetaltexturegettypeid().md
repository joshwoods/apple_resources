

- Core Video
-  CVMetalTextureGetTypeID() 

Function

# CVMetalTextureGetTypeID()

Returns the Core Foundation type identifier for a CoreVideo Metal texture-based image buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func CVMetalTextureGetTypeID() -> CFTypeID
```

## Return Value

The Core Foundation type identifier for the `CVMetalTextureRef` type.

## See Also

### Related Documentation

Metal Programming Guide

Metal

Render advanced 3D graphics and compute data in parallel with graphics processors.

### Inspecting Textures

func CVMetalTextureGetTexture(CVMetalTexture) -> (any MTLTexture)?

Returns the Metal texture object for the image buffer.

func CVMetalTextureGetCleanTexCoords(CVMetalTexture, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

Returns convenient normalized texture coordinates for the part of the image that should be displayed.

func CVMetalTextureIsFlipped(CVMetalTexture) -> Bool

Returns a Boolean value indicating whether the texture image is vertically flipped.

