

- Core Image
-  CIKernel 

Class

# CIKernel

A GPU-based image-processing routine used to create custom Core Image filters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class CIKernel : NSObject
```

## Overview

Note

If your custom filter uses both color and geometry information, but does not require processing both at the same time, you can improve performance by separating your image processing code: use a CIColorKernel object for the color processing step and a CIWarpKernel object for the geometry processing step.

The kernel language routine for a general-purpose filter kernel has the following characteristics:

- Its return type is `vec4` (Core Image Kernel Language) or `float4` (Metal Shading Language); that is, it returns a pixel color for the output image.

- It may use zero or more input images. Each input image is represented by a parameter of type `sampler`.

A kernel routine typically produces its output by calculating source image coordinates (using the `destCoord` and `samplerTransform` functions or the `samplerTransform` function), samples from the source images (using the `sample` function), and computes a final pixel color (output using the `return` keyword). For example, the Metal Shading Language source below implements a filter that passes through its input image unchanged.

#include &lt;CoreImage/CoreImage.h>

extern &quot;C&quot; {
    namespace coreimage {
        float4 do_nothing(sampler src) {
            return src.sample(src.coord());
        }
    }
}

The equivalent code in Core Image Kernel Language is:

kernel vec4 do_nothing(sampler image) {
    vec2 dc = destCoord();
    return sample(image, samplerTransform(image, dc));
}

The Core Image Kernel Language is a dialect of the OpenGL Shading Language. See Core Image Kernel Language Reference and Core Image Programming Guide for more details.

## Topics

### Creating a Kernel Using Metal Shading Language

init(functionName: String, fromMetalLibraryData: Data)

Creates a single kernel object using a Metal Shading Language (MSL) kernel function.

init(functionName: String, fromMetalLibraryData: Data, outputPixelFormat: CIFormat)

Creates a single kernel object using a Metal Shading Language kernel function with optional pixel format.

class func kernelNames(fromMetalLibraryData: Data) -> [String]

Return an array of strings containing the names of all of the kernels contained in the Metal library.

class func kernels(withMetalString: String) -> [CIKernel]

Load kernels from a Metal language string.

### Getting a Kernel Name

var name: String

The name of the kernel routine.

### Identifying the Region of Interest for the Kernel

func setROISelector(Selector)

Sets the selector Core Image uses to query the region of interest for image processing with the kernel.

### Applying a Kernel to Filter an Image

func apply(extent: CGRect, roiCallback: CIKernelROICallback, arguments: [Any]) -> CIImage?

Creates a new image using the kernel and specified arguments.

typealias CIKernelROICallback

The signature for a block that computes the region of interest (ROI) for a given area of destination image pixels. Core Image calls this block when applying the kernel. You specify this block when using the apply(extent:roiCallback:arguments:) method.

### Deprecated

init?(source: String)

Creates a single kernel object.

Deprecated

class func makeKernels(source: String) -> [CIKernel]?

Creates and returns and array of `CIKernel` objects.

Deprecated

## Relationships

### Inherits From

- NSObject

## See Also

### Custom Filters

Writing Custom Kernels

Write your own custom kernels in either the Core Image Kernel Language or the Metal Shading Language.

class CIColorKernel

A GPU-based image-processing routine that processes only the color information in images, used to create custom Core Image filters.

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

