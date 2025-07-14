

- Metal
- Textures
-  Creating a Mipmapped Texture 

Article

# Creating a Mipmapped Texture

Decide whether a texture that you’re creating needs mipmaps.

## Overview

In Metal, the same MTLTexture object owns all of the mipmaps for a texture. When you create the texture descriptor for a new texture, you determine many of the texture’s fixed properties, including how many mipmaps it has. Set the mipmapLevelCount property to the number of mipmap levels you want the texture to have. The default value is `1`, which means that Metal doesn’t create mipmaps.

The code below creates a texture with multiple mipmaps. It calculates the number of mipmaps needed for a full mipmap chain, from the original size down to a `1x1` texture, and sets that number as the mipmap count. Generating a full mipmap chain requires 33% more memory than if you just had the top image. You can choose to create a mipmap chain that has fewer mipmap levels.

- Swift
- Objective-C

```
/// Create a mipmap texture.
func makeMipTexture(for device: MTLDevice, with size: MTLSize) -> MTLTexture? {
    let descriptor = MTLTextureDescriptor()

    descriptor.width = size.width
    descriptor.height = size.height
    descriptor.depth = size.depth

    let heightLevels = ceil(log2(Double(size.height)))
    let widthLevels = ceil(log2(Double(size.width)))
    let mipCount = (heightLevels > widthLevels) ? heightLevels : widthLevels

    descriptor.mipmapLevelCount = Int(mipCount)

    return device.makeTexture(descriptor: descriptor)
}
```

```
/// Create a mipmap texture.
- (id) makeMipTextureWithSize: (MTLSize) size
{
    MTLTextureDescriptor *descriptor = [MTLTextureDescriptor new];
    ...
    descriptor.width = size.width;
    descriptor.height = size.height;
    descriptor.depth = size.depth;

    int heightLevels = ceil(log2(size.height));
    int widthLevels = ceil(log2(size.width));
    int mipCount = (heightLevels > widthLevels) ? heightLevels : widthLevels;

    descriptor.mipmapLevelCount = mipCount;

    return [_device newTextureWithDescriptor: descriptor];
}
```

When you create a texture, Metal doesn’t initialize mipmap levels. You need to provide data for any mipmap levels that the GPU accesses. Further, Metal doesn’t keep track of which mipmaps you’ve filled in, or which contain uninitialized or stale data. You’ll need to keep track of that information yourself.

### Load a Mipmapped Texture Using MetalKit

If you use MetalKit to create a texture, and the source data includes multiple mipmaps, MetalKit automatically creates the texture with the correct number of mipmaps and copies the source data into the appropriate mipmap levels. If the source data doesn’t include mipmaps, MetalKit creates a texture with just one texture image.

You can override this behavior by providing an options dictionary with one of the following keys:

- The allocateMipmaps key with a value of true allocates a full set of mipmap levels for the texture. After loading is complete, Metal fills mipmap `0` with the source data, and leaves the other mipmap contents uninitialized; you fill the other mipmaps with data. Similarly, if you provide this key with a value of false, Metal ignores any extra mipmap data and only loads the top mipmap.

- The generateMipmaps key with a value of true allocates a full set of mipmap levels for the texture. This key has the device object generate images for the lower-level mipmaps by filtering the provided source data.

## See Also

### Texture Mipmapping

Improving Texture Sampling Quality and Performance with Mipmaps

Avoid texture-rendering artifacts and reduce the GPU’s workload by creating smaller versions of a texture.

Copying Data into or out of Mipmaps

Specify which mipmaps that the data transfer affects.

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

