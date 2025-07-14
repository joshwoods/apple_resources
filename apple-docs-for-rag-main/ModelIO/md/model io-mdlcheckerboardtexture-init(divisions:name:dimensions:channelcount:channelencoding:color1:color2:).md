

- Model I/O
- MDLCheckerboardTexture
-  init(divisions:name:dimensions:channelCount:channelEncoding:color1:color2:) 

Initializer

# init(divisions:name:dimensions:channelCount:channelEncoding:color1:color2:)

Initializes a checkerboard texture with the specified colors and other properties.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    divisions: Float,
    name: String?,
    dimensions: vector_int2,
    channelCount: Int32,
    channelEncoding: MDLTextureChannelEncoding,
    color1: CGColor,
    color2: CGColor
)
```

## Parameters 

`divisions`  

The number of squares along each dimension in the checkerboard pattern.

`name`  

The name property for the new texture object.

`dimensions`  

The texel dimensions (width and height) of the texture image.

`channelCount`  

The number of channels per texel—for example, 1 for a grayscale texture, 3 for an RGB color texture, or 4 for RGBA.

`channelEncoding`  

The data format for each channel value per texel—for example, 8-bit integer or 32-bit floating point. For possible values, see MDLTextureChannelEncoding.

`color1`  

The color for half of the squares in the checkerboard pattern.

`color2`  

The color for the other half of the squares in the checkerboard pattern.

## Return Value

A new checkerboard texture object.

## Discussion

The `divisions`, `color1`, and `color2` parameters define the checkerboard pattern. For example, a `divisions` value of 2 creates a checkerboard pattern of four squares (a 2 x 2 grid), where the top left and bottom right squares use the `color1` color and the other two squares use the `color2` color. A value of 4 creates a pattern of 16 squares (a 4 x 4 grid), and so on.

This initializer does not generate texel data; the MDLCheckerboardTexture class automatically generates data and caches it for reuse when you use one of the MDLTexture methods listed in Accessing Texture Data. Changing the divisions, color1, or color2 properties invalidates the cache, causing Model I/O to regenerate texel data the next time it is needed.

