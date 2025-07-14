

- Core Image
-  CIFilterShape 

Class

# CIFilterShape

A description of the bounding shape of a filter and the domain of definition for a filter operation.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class CIFilterShape : NSObject
```

## Overview

You use `CIFilterShape` objects in conjunction with Core Image classes, such as CIFilter, CIKernel, and CISampler, to create custom filters.

## Topics

### Initializing a Filter Shape

init(rect: CGRect)

Initializes a filter shape object with a rectangle.

### Inspecting a Filter Shape

var extent: CGRect

The extent of the filter shape.

### Modifying a Filter Shape

func insetBy(x: Int32, y: Int32) -> CIFilterShape

Modifies a filter shape object so that it is inset by the specified x and y values.

func intersect(with: CIFilterShape) -> CIFilterShape

Creates a filter shape object that represents the intersection of the current filter shape and the specified filter shape object.

func intersect(with: CGRect) -> CIFilterShape

Creates a filter shape that represents the intersection of the current filter shape and a rectangle.

func transform(by: CGAffineTransform, interior: Bool) -> CIFilterShape

Creates a filter shape that results from applying a transform to the current filter shape.

func union(with: CIFilterShape) -> CIFilterShape

Creates a filter shape that results from the union of the current filter shape and another filter shape object.

func union(with: CGRect) -> CIFilterShape

Creates a filter shape that results from the union of the current filter shape and a rectangle.

## Relationships

### Inherits From

- NSObject

### Conforms To

- NSCopying

## See Also

### Custom Filters

Writing Custom Kernels

Write your own custom kernels in either the Core Image Kernel Language or the Metal Shading Language.

class CIKernel

A GPU-based image-processing routine used to create custom Core Image filters.

class CIColorKernel

A GPU-based image-processing routine that processes only the color information in images, used to create custom Core Image filters.

class CIWarpKernel

A GPU-based image-processing routine that processes only the geometry information in an image, used to create custom Core Image filters.

class CIBlendKernel

A GPU-based image-processing routine that is optimized for blending two images.

class CISampler

An object that retrieves pixel samples for processing by a filter kernel.

struct CIFormat

Pixel data formats for image input, output, and processing.

