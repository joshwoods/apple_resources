

- Metal
- Textures
-  Predicting Which Mips the GPU Samples with Level-of-Detail Queries 

Article

# Predicting Which Mips the GPU Samples with Level-of-Detail Queries

Determine in advance which mipmap levels the GPU requires to sample a texture.

## Overview

When you sample a texture, the GPU automatically chooses which mipmaps to access and fetches pixels from them. Each mipmap represents a different level-of-detail (LOD).

Sometimes, you want to know which mipmaps the GPU would read from. For example, if only some of your mipmaps have data, you might use a clamp operation to limit the range of mipmaps the GPU can sample from, but want to know when the GPU requires sampling higher mipmaps. Metal Shading Language provides texture functions that you can use to determine which mipmaps your shader would access if it were to sample the texture.

### Check for Level-of-Detail Support

Before loading any shaders that use LOD queries, make sure the GPU supports them by checking if it supports one of the following:

- The MTLGPUFamily.mac2 feature set.

- The MTLGPUFamily.apple7 feature set.

- Swift
- Objective-C

```
let macFamily2Support = device.supportsFamily(MTLGPUFamily.mac2)
let appleFamily7Support = device.supportsFamily(MTLGPUFamily.apple7)
let supportsCalculateLevelOfDetail = macFamily2Support || appleFamily7Support
```

```
Boolean macFamily2Support = [device supportsFamily: MTLGPUFamilyMac2];
Boolean appleFamily7Support = [device supportsFamily: MTLGPUFamilyApple7];
Boolean supportsCalculateLevelOfDetail = macFamily2Support || appleFamily7Support;
```

### Determine Level of Detail

In your shader, the functions that return LOD information have signatures that are similar to those of functions used to sample textures. There are two kinds of these functions: clamped and unclamped. The clamped kind restricts LOD selection by applying the sampler’s range of permitted values, the range of mipmaps provided in the texture, and the sampler’s anisotropy settings. The unclamped kind returns the raw calculation.

```
float clampedLOD = texture.calculate_clamped_lod(mySampler, coords);
float unclampedLOD = texture.calculate_unclamped_lod(mySampler, coords);
```

A fractional part in a returned value indicates that the value is between two mipmaps. The fractional part of the number is the blending weight between the two mipmaps if you’ve specified linear mipmap blending.

### Determine Level of Detail When Shader Support is Unavailable

Alternatively, you can get the LOD by performing the calculation yourself, based on the size of the model object and its distance from the camera. For an example of this technique, see Using Function Specialization to Build Pipeline Variants.

## See Also

### Texture Mipmapping

Improving Texture Sampling Quality and Performance with Mipmaps

Avoid texture-rendering artifacts and reduce the GPU’s workload by creating smaller versions of a texture.

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

Dynamically Adjusting Texture Level of Detail

Defer generating or loading larger mipmaps until that level of detail is needed.

