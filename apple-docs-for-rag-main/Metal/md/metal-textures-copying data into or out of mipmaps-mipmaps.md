

- Metal
- Textures
-  Copying Data into or out of Mipmaps 

Article

# Copying Data into or out of Mipmaps

Specify which mipmaps that the data transfer affects.

## Overview

When you copy data between resources, and the source or destination is a texture, specify which mipmaps that the data transfer affects.

### Copy Data from System Memory to a Mipmap

When you copy data from system memory into a texture, using the replace(region:mipmapLevel:withBytes:bytesPerRow:) or similar method, state which mipmap is the destination of that copy.

- Swift
- Objective-C

```
// Create a 3D region, where image is a CGContext object.
let image = 
let region: MTLRegion = MTLRegionMake3D(0, 0, 0, image.width, image.height, 1)

// Replace the region in the texture.
texture.replace(region: region, mipmapLevel: 0, withBytes: image.data!, bytesPerRow: image.bytesPerRow)
```

```
MTLRegion region = {
    { 0, 0, 0 },                   // MTLOrigin
    {image.width, image.height, 1} // MTLSize
};

[texture replaceRegion:region
           mipmapLevel:0
             withBytes:image.data.bytes
           bytesPerRow:bytesPerRow];
```

Call this routine once for each mipmap you want to fill, changing the region to match the size of the mipmap level you’re writing to.

### Copy Mipmap Data Between Metal Resources

If you already have data in Metal resources, use a MTLBlitCommandEncoder to copy data to and from different mipmaps in a texture.

To copy all matching data between two textures, encode a command using the copy(from:to:): method. The two textures must have the same pixel format and type. Metal copies all matching mipmap sizes to the destination texture.

To copy a selection of mipmaps from one texture to another, use the copy(from:sourceSlice:sourceLevel:to:destinationSlice:destinationLevel:sliceCount:levelCount:) method. Specify the first source mipmap level and first destination mipmap level, both of which must have the same dimensions. Also specify the number of mipmap levels you want to copy.

For example, the following code assumes that the destination texture is twice as large in both dimensions as the source texture. Mipmap `1` in the destination matches the size of the source mipmap `0`, so the code passes `0` as the source level and `1` as the destination level. It also passes `5` as the level count to copy `5` mipmaps.

- Swift
- Objective-C

```
// Copy mipmap data between MTLTexture objects.
let source = , destination = 

encoder.copy(from: source, sourceSlice: 0, sourceLevel: 0, to: destination, destinationSlice: 0,
             destinationLevel: 1, sliceCount: 1, levelCount: 5)
```

```
[encoder copyFromTexture: source
    sourceSlice: 0
    sourceLevel: 0
    toTexture: destination
    destinationSlice: 0
    destinationLevel: 1
    sliceCount: 1
    levelCount: 5];
```

If you need to copy data between buffers and textures, encode a separate blit command for each mipmap level to copy. See MTLBlitCommandEncoder for other methods that copy data to and from textures.

## See Also

### Texture Mipmapping

Improving Texture Sampling Quality and Performance with Mipmaps

Avoid texture-rendering artifacts and reduce the GPU’s workload by creating smaller versions of a texture.

Creating a Mipmapped Texture

Decide whether a texture that you’re creating needs mipmaps.

Generating Mipmap Data

Create your mipmaps either when you author content or at runtime.

Adding Mipmap Filtering to Samplers

Specify how the GPU samples mipmaps in your textures.

Restricting Access to Specific Mipmaps

Set the range of mipmap levels that a sampler can access.

Predicting Which Mips the GPU Samples with Level-of-Detail Queries

Determine in advance which mipmap levels the GPU requires to sample a texture.

Dynamically Adjusting Texture Level of Detail

Defer generating or loading larger mipmaps until that level of detail is needed.

