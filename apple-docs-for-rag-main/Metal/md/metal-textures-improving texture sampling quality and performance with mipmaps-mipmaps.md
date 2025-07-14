

- Metal
- Textures
-  Improving Texture Sampling Quality and Performance with Mipmaps 

Article

# Improving Texture Sampling Quality and Performance with Mipmaps

Avoid texture-rendering artifacts and reduce the GPU’s workload by creating smaller versions of a texture.

## Overview

*Mipmaps* are progressively smaller versions of the same texture image, each of which provides a different level of detail (LOD) for the texture. A texture’s *mipmap chain* is its complete set of mipmaps. Textures with mipmaps can help your app eliminate common visual problems, such as aliasing and moire patterns, while reducing the GPU’s memory bandwidth.

\_\_The largest version of a texture is mipmap `0` and it’s at the top of the mipmap chain. The next largest version is mipmap `1`, which is one level lower in the chain.

Each nonzero mipmap level is 25% of the area of the previous mipmap level in the chain. A texture’s smallest mipmap is at least 1 pixel in each dimension.

A mipmapped texture gives the GPU the option to sample from a mipmap size that’s closest to the size of the primitive it’s rendering to. A GPU’s texture-sampling hardware works best when a texture’s dimensions are similar to the output primitive’s dimensions. Without mipmaps, the GPU can sample only the full-size texture, including when an output primitive is much smaller than the texture. In that scenario, the hardware typically fetches a significant portion of the texture to properly filter for color.

For example, to filter a 256 x 256 texture to an 8 x 8 rendering, the GPU needs to blend 25% of the texture for each output pixel. Additionally, you can’t precisely control which pixels the GPU fetches from the texture and then blends to render to a relatively small primitive. That imprecision can produce an obviously incorrect image, especially when it spans multiple frames, such as during animations.

Mipmapped textures can also help improve your app’s performance because a GPU uses less memory bandwidth and memory cache by sampling from the smaller mipmaps.

You can create a mipmapped texture and initialize its mipmap chain by following the steps in Creating a Mipmapped Texture and Generating Mipmap Data, respectively.

## See Also

### Texture Mipmapping

Creating a Mipmapped Texture

Decide whether a texture that you’re creating needs mipmaps.

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

