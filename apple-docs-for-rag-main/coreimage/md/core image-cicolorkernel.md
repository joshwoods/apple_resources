

- Core Image
-  CIColorKernel 

Class

# CIColorKernel

A GPU-based image-processing routine that processes only the color information in images, used to create custom Core Image filters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class CIColorKernel : CIKernel
```

## Overview

The kernel language routine for a color kernel has the following characteristics:

- Its return type is `vec4` (Core Image Kernel Language) or `float4` (Metal Shading Language); that is, it returns a pixel color for the output image.

- It may use zero or more input images. Each input image is represented by a parameter of type `__sample` (Core Image Kernel Language) or `sample_t` (Metal Shading Language), which can be treated as a single pixel color of type `vec4` (Core Image Kernel Language) or `float4` (Metal Shading Language);.

A color kernel routine receives as input single-pixel colors (one sampled from each input image) and computes a final pixel color (output using the `return` keyword). For example, the Metal Shading Language source below implements a filter that passes through its input image unchanged.

#include &lt;CoreImage/CoreImage.h>

extern &quot;C&quot; {
    namespace coreimage {
        float4 do_nothing(sample_t s) {
            return s;
        }
    }
}

The equivalent code in Core Image Kernel Language is:

kernel vec4 do_nothing(__sample s) {
    return s.rgba;
}

The Core Image Kernel Language is a dialect of the OpenGL Shading Language. See Core Image Kernel Language Reference and Core Image Programming Guide for more details.

## Topics

### Creating a Kernel

init?(source: String)

Creates a color kernel object from the specified kernel source code.

Deprecated

### Applying a Kernel to Filter an Image

func apply(extent: CGRect, arguments: [Any]) -> CIImage?

Creates a new image using the kernel and specified arguments.

## Relationships

### Inherits From

- CIKernel

## See Also

### Custom Filters

Writing Custom Kernels

Write your own custom kernels in either the Core Image Kernel Language or the Metal Shading Language.

class CIKernel

A GPU-based image-processing routine used to create custom Core Image filters.

class CIWarpKernel

A GPU-based image-processing routine that processes only the geometry information in an image, used to create custom Core Image filters.

class CIBlendKernel

A GPU-based image-processing routine that is optimized for blending two images.

class CISampler

An object that retrieves pixel samples for processing by a filter kernel.

class CIFilterShape

A description of the bounding shape of a filter and the domain of definition for a filter operation.

struct CIFormat

Pixel data formats for image input, output, and processing.

