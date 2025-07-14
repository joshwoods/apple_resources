

- Metal
- MTLResourceStateCommandEncoder
-  moveTextureMappings(sourceTexture:sourceSlice:sourceLevel:sourceOrigin:sourceSize:destinationTexture:destinationSlice:destinationLevel:destinationOrigin:) 

Instance Method

# moveTextureMappings(sourceTexture:sourceSlice:sourceLevel:sourceOrigin:sourceSize:destinationTexture:destinationSlice:destinationLevel:destinationOrigin:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

**iOS, iPadOS, tvOS, visionOS**

``` source
func moveTextureMappings(
    sourceTexture: any MTLTexture,
    sourceSlice: Int,
    sourceLevel: Int,
    sourceOrigin: MTLOrigin,
    sourceSize: MTLSize,
    destinationTexture: any MTLTexture,
    destinationSlice: Int,
    destinationLevel: Int,
    destinationOrigin: MTLOrigin
)
```

**Mac Catalyst, macOS**

``` source
optional func moveTextureMappings(
    sourceTexture: any MTLTexture,
    sourceSlice: Int,
    sourceLevel: Int,
    sourceOrigin: MTLOrigin,
    sourceSize: MTLSize,
    destinationTexture: any MTLTexture,
    destinationSlice: Int,
    destinationLevel: Int,
    destinationOrigin: MTLOrigin
)
```

**Required**

