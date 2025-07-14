

- Core Image
- CIFilter
-  Options for Applying a Filter 

API Collection

# Options for Applying a Filter

Options that control the application of a custom Core Image filter.

## Overview

Use these constants only when creating a custom filter for which you are writing the kernel. For more information, see Core Image Programming Guide. The example on creating a custom filter shows how to use these options.

## Topics

### Constants

let kCIApplyOptionExtent: String

The size of the produced image. The associated value is a four-element array (NSArray) that specifies the x-value of the rectangle origin, the y-value of the rectangle origin, and the width and height.

let kCIApplyOptionDefinition: String

The domain of definition (DOD) of the produced image. The associated value is either a Core Image filter shape or a four-element array (NSArray) that specifies a rectangle.

let kCIApplyOptionUserInfo: String

Information needed by a callback. The associated value is an object that Core Image will pass to any callbacks invoked for that filter.

let kCIApplyOptionColorSpace: String

The color space of the produced image. The associated value must be an RGB CGColorSpace object. If not specified, the output of the kernel is in the working color space of the Core Image context used to render the image.

