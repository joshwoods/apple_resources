

- Core Image
-  CIWarpKernel 

Class

# CIWarpKernel

A GPU-based image-processing routine that processes only the geometry information in an image, used to create custom Core Image filters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class CIWarpKernel : CIKernel
```

## Overview

The kernel language routine for a warp kernel has the following characteristics:

- It uses exactly one input image.

- Its return type is `vec2 `(Core Image Kernel Language) or `float2` (Metal Shading Language), specifying a position in source image coordinates.

A warp kernel routine requires no input parameters (but can use additional custom parameters you declare). Typically, a warp kernel uses the destination coordinate function to look up the coordinates of the destination pixel currently being rendered, then computes a corresponding position in source image coordinates (output using the `return` keyword). Core Image then samples from the source image at the returned coordinates to produce a pixel color for the output image. For example, the Metal Shading Language source below implements a filter that passes through its input image unchanged.

#include &lt;CoreImage/CoreImage.h>

extern &quot;C&quot; {
    namespace coreimage {
        float2 do_nothing(destination dest) {
            return dest.coord();
        }
    }
}

The equivalent code in Core Image Kernel Language is:

kernel vec2 do_nothing() {
    return destCoord();
}

The Core Image Kernel Language is a dialect of the OpenGL Shading Language. See Core Image Kernel Language Reference and Core Image Programming Guide for more details.

## Topics

### Creating a Kernel

init?(source: String)

Creates a warp kernel object from the specified kernel source code.

Deprecated

### Applying a Kernel to Filter an Image

func apply(extent: CGRect, roiCallback: CIKernelROICallback, image: CIImage, arguments: [Any]) -> CIImage?

Creates a new image using the kernel and the specified input image and arguments.

## Relationships

### Inherits From

- CIKernel

## See Also

### Custom Filters

Writing Custom Kernels

Write your own custom kernels in either the Core Image Kernel Language or the Metal Shading Language.

class CIKernel

A GPU-based image-processing routine used to create custom Core Image filters.

class CIColorKernel

A GPU-based image-processing routine that processes only the color information in images, used to create custom Core Image filters.

class CIBlendKernel

A GPU-based image-processing routine that is optimized for blending two images.

class CISampler

An object that retrieves pixel samples for processing by a filter kernel.

class CIFilterShape

A description of the bounding shape of a filter and the domain of definition for a filter operation.

struct CIFormat

Pixel data formats for image input, output, and processing.

