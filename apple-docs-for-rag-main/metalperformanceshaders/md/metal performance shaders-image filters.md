

- Metal Performance Shaders
-  Image Filters 

API Collection

# Image Filters

Apply high-performance filters to, and extract statistical and histogram data from images.

## Overview

The MPSUnaryImageKernel and MPSBinaryImageKernel base classes define several properties common to all image kernels:

|  |  |
|----|----|
| clipRect and clipRect | A clip rectangle is available to all image kernels that write to a destination texture. It describes the sub-rectangle of the destination texture overwritten by the filter. If the clip rectangle is larger than the destination texture, then the intersection between the clip rectangle and the destination texture bounds is used instead. A clip rectangle may be used to avoid doing work to obscured regions of the destination image, or to manage tiling and limit operations to parts of an image—for example, if a user draws a rectangle on the screen and asks your app to just apply the filter there. |
| offset, primaryOffset, and secondaryOffset | An offset is available to all image kernels that use a source texture from which pixel data is read. It describes the positioning of the source image relative to the result texture. An offset of `{0, 0, 0}` indicates that the top left pixel of the source texture is the center pixel used to create the top left corner of the destination texture clip rectangle (as a further example, an offset of `{1, 2, 0}` positions the top left corner of the clip rectangle at position `x=1`, `y=2`, and `z=0` of the source image). The offset is the position of the top left corner of the clip rectangle in the source coordinate frame. It can be used for tiling and for translating an image up, down, left, or right by pixel increments. If there is no clip rectangle, then the offset is the top left corner of the region read by the filter. If there are multiple source textures, then the primary offset describes the top left corner of the region read in the primary source texture and the secondary offset describes the top left corner of the region read in the secondary source texture. |
| edgeMode, primaryEdgeMode, and secondaryEdgeMode | An edge mode describes the behavior of texture reads that stray off the edge of the source image. This can happen if the offset is negative, meaning a read off the top or left edge of the image. This can also happen if the sum of the clip rectangle size and the offset is larger than the source image, meaning a read off the bottom or right edge of the image. Furthermore, it is also possible for image filters to have a kernel window that stretches to examine neighboring pixels beyond the image bounds (such as convolution, morphology, and resampling filters). If there are multiple source textures, then the primary edge mode describes the mode to use with the primary source texture and the secondary edge mode describes the mode to use with the secondary source texture. |

### In-Place Operation

Some kernels can operate in place. This means that the same texture is used to hold both the input image and the result image. Operating in place is a great way to save memory, time, and energy. You can perform an in-place operation by using the encode(commandBuffer:inPlaceTexture:fallbackCopyAllocator:) method.

Unfortunately, it is not always possible for kernels to run in place. Whether a particular kernel can operate in place can vary according to the hardware it is running on, the OS version, and the parameters and properties passed to it. You may not assume that because a kernel works in place today on a particular device that it will do so in the future.

To simplify error handling with failed in-place operation, the encode(commandBuffer:inPlaceTexture:fallbackCopyAllocator:) method takes an optional MPSCopyAllocator object. It is used to create a new texture when in-place operation is not possible so as to allow the operation to proceed out of place in a reliable fashion instead. When this happens, the input texture is released and replaced with a new texture. To make use of the feature, you will need to write a copy allocator block.

Listing 1 shows a minimal copy allocator implementation. For more information, see the MPSCopyAllocator reference.

Listing 1 Minimal MPSCopyAllocator Implementation

### Supported Pixel Formats for Image Kernels

All Metal Performance Shaders image kernels support source and destination textures with the following ordinary and packed pixel formats:

MTLPixelFormat.r8Unorm, MTLPixelFormat.r8Unorm_srgb  
Ordinary formats with one 8-bit normalized unsigned integer component.

MTLPixelFormat.rg8Unorm, MTLPixelFormat.rg8Unorm_srgb  
Ordinary formats with two 8-bit normalized unsigned integer components.

MTLPixelFormat.rgba8Unorm, MTLPixelFormat.rgba8Unorm_srgb, MTLPixelFormat.bgra8Unorm, MTLPixelFormat.bgra8Unorm_srgb  
Ordinary formats with four 8-bit normalized unsigned integer components.

MTLPixelFormat.r16Float, MTLPixelFormat.rg16Float, MTLPixelFormat.rgba16Float  
Ordinary format with 16-bit floating-point components.

MTLPixelFormat.r32Float, MTLPixelFormat.rg32Float, MTLPixelFormat.rgba32Float  
Ordinary format with 32-bit floating-point components.

MTLPixelFormat.r16Unorm, MTLPixelFormat.rg16Unorm, MTLPixelFormat.rgba16Unorm  
Ordinary format with 16-bit normalized unsigned integer components.

MTLPixelFormat.b5g6r5Unorm, MTLPixelFormat.a1bgr5Unorm, MTLPixelFormat.abgr4Unorm, MTLPixelFormat.bgr5A1Unorm  
Packed 16-bit format with normalized unsigned integer color components.

MTLPixelFormat.rgb10a2Unorm  
Packed 32-bit format with normalized unsigned integer color components.

MTLPixelFormat.rg11b10Float, MTLPixelFormat.rgb9e5Float  
Packed 32-bit format with floating-point color components.

Some compressed pixel formats can be used as source textures. They cannot be used as destination textures because they cannot be written to. Metal Performance Shaders image kernels support the following compression families:

- PVRTC

- EAC/ETC

- ASTC

The following Metal Performance Shaders image kernels also support source and destination textures with ordinary signed and unsigned integer pixel formats:

- MPSImageTranspose

- MPSImageIntegral

- MPSImageIntegralOfSquares

The ordinary signed and unsigned integer pixel formats supported by these image kernels:

MTLPixelFormat.r8Sint, MTLPixelFormat.rg8Sint, MTLPixelFormat.rgba8Sint  
Ordinary format with 8-bit signed integer components.

MTLPixelFormat.r8Uint, MTLPixelFormat.rg8Uint, MTLPixelFormat.rgba8Uint  
Ordinary format with 8-bit unsigned integer components.

MTLPixelFormat.r16Sint, MTLPixelFormat.rg16Sint, MTLPixelFormat.rgba16Sint  
Ordinary format with 16-bit signed integer components.

MTLPixelFormat.r16Uint, MTLPixelFormat.rg16Uint, MTLPixelFormat.rgba16Uint  
Ordinary format with 16-bit unsigned integer components.

MTLPixelFormat.r32Sint, MTLPixelFormat.rg32Sint, MTLPixelFormat.rgba32Sint  
Ordinary format with 32-bit signed integer components.

MTLPixelFormat.r32Uint, MTLPixelFormat.rg32Uint, MTLPixelFormat.rgba32Uint  
Ordinary format four 32-bit unsigned integer components.

For more information on pixel formats, see MTLPixelFormat and Pixel Format Capabilities.

### Sample Code

Listing 2 Metal Performance Shaders Sample Code

## Topics

### Morphological Image Filters

class MPSImageAreaMax

A filter that finds the maximum pixel value in a rectangular region centered around each pixel in the source image.

class MPSImageDilate

A filter that finds the maximum pixel value in a rectangular region by applying a dilation function.

class MPSImageAreaMin

A filter that finds the minimum pixel value in a rectangular region centered around each pixel in the source image.

class MPSImageErode

A filter that finds the minimum pixel value in a rectangular region by applying an erosion function.

### Convolution Image Filters

class MPSImageConvolution

A filter that convolves an image with a given kernel of odd width and height.

class MPSImageMedian

A filter that applies a median filter in a square region centered around each pixel in the source image.

class MPSImageBox

A filter that convolves an image with a given kernel of odd width and height.

class MPSImageTent

A filter that convolves an image with a tent filter.

class MPSImageGaussianBlur

A filter that convolves an image with a Gaussian blur of a given sigma in both the x and y directions.

class MPSImageGaussianPyramid

A filter that convolves an image with a Gaussian pyramid.

class MPSImageSobel

A filter that convolves an image with the Sobel operator.

class MPSImageLaplacian

An optimized Laplacian filter, provided for ease of use.

class MPSImageLaplacianPyramid

A filter that convolves an image with a Laplacian filter.

class MPSImageLaplacianPyramidAdd

A filter that convolves an image with an additive Laplacian pyramid.

class MPSImageLaplacianPyramidSubtract

A filter that convolves an image with a subtractive Laplacian pyramid.

class MPSImagePyramid

A base class for creating different kinds of pyramid images.

### Histogram Image Filters

class MPSImageHistogram

A filter that computes the histogram of an image.

class MPSImageHistogramEqualization

A filter that equalizes the histogram of an image.

class MPSImageHistogramSpecification

A filter that performs a histogram specification operation on an image.

### Image Threshold Filters

class MPSImageThresholdBinary

A filter that returns a specified value for each pixel with a value greater than a specified threshold or 0 otherwise.

class MPSImageThresholdBinaryInverse

A filter that returns 0 for each pixel with a value greater than a specified threshold or a specified value otherwise.

class MPSImageThresholdToZero

A filter that returns the original value for each pixel with a value greater than a specified threshold or 0 otherwise.

class MPSImageThresholdToZeroInverse

A filter that returns 0 for each pixel with a value greater than a specified threshold or the original value otherwise.

class MPSImageThresholdTruncate

A filter that clamps the return value to an upper specified value.

### Image Integral Filters

class MPSImageIntegral

A filter that calculates the sum of pixels over a specified region in an image.

class MPSImageIntegralOfSquares

A filter that calculates the sum of squared pixels over a specified region in an image.

### Image Manipulation Filters

class MPSImageConversion

A filter that performs a conversion of color space, alpha, or pixel format.

class MPSImageScale

A filter that resizes and changes the aspect ratio of an image.

class MPSImageLanczosScale

A filter that resizes and changes the aspect ratio of an image using Lanczos resampling.

class MPSImageBilinearScale

A filter that resizes and changes the aspect ratio of an image using Bilinear resampling.

class MPSImageTranspose

A filter that transposes an image.

### Image Statistics Filters

class MPSImageStatisticsMean

A kernel that computes the mean for a given region of an image.

class MPSImageStatisticsMeanAndVariance

A kernel that computes the mean and variance for a given region of an image.

class MPSImageStatisticsMinAndMax

A kernel that computes the minimum and maximum pixel values for a given region of an image.

### Image Reduction Filters

class MPSImageReduceRowMax

A filter that returns the maximum value for each row in an image.

class MPSImageReduceRowMin

A filter that returns the minimum value for each row in an image.

class MPSImageReduceRowSum

A filter that returns the sum of all values for a row in an image.

class MPSImageReduceRowMean

A filter that returns the mean value for each row in an image.

class MPSImageReduceColumnMax

A filter that returns the maximum value for each column in an image.

class MPSImageReduceColumnMin

A filter that returns the minimum value for each column in an image.

class MPSImageReduceColumnSum

A filter that returns the sum of all values for a column in an image.

class MPSImageReduceColumnMean

A filter that returns the mean value for each column in an image.

class MPSImageReduceUnary

The base class for reduction filters that take a single source as input.

### Image Arithmetic Filters

class MPSImageAdd

A filter that returns the element-wise sum of its two input images.

class MPSImageSubtract

A filter that returns the element-wise difference of its two input images.

class MPSImageMultiply

A filter that returns the element-wise product of its two input images.

class MPSImageDivide

A filter that returns the element-wise quotient of its two input images.

class MPSImageArithmetic

Base class for basic arithmetic nodes

### Euclidean Distance Transform Filter

class MPSImageEuclideanDistanceTransform

A filter that performs a Euclidean distance transform on an image.

### Fast Guided Filter

class MPSImageGuidedFilter

A filter that performs edge-aware filtering on an image.

### Keypoints

class MPSImageFindKeypoints

A kernel that is used to find a list of keypoints.

struct MPSImageKeypointData

A structure that specifies keypoint information.

struct MPSImageKeypointRangeInfo

A structure that specifies information to find the keypoints in an image.

### Image Filter Base Classes

class MPSUnaryImageKernel

A kernel that consumes one texture and produces one texture.

class MPSBinaryImageKernel

A kernel that consumes two textures and produces one texture.

### Constants

MPSRectNoClip

The default clipping rectangle for a kernel object.

