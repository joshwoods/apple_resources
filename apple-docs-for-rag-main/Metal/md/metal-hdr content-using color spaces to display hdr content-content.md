

- Metal
- HDR Content
-  Using Color Spaces to Display HDR Content 

Article

# Using Color Spaces to Display HDR Content

Use a color space when you don’t need to edit or process the pixel data.

## Overview

If you aren’t editing the content in a linear color space, and simply need to display the content with the correct transfer function, use a color space that includes that transfer function. Create a Metal layer and set its wantsExtendedDynamicRangeContent property to true. Set the color space that matches the color primaries and transfer function of your content. The code below creates a Metal layer for content in the BT.2020 color space using the PQ transfer function:

- Swift
- Objective-C

```
let metalLayer = CAMetalLayer()
metalLayer.wantsExtendedDynamicRangeContent = true
metalLayer.pixelFormat = .bgr10a2Unorm
let name = CGColorSpace.itur_2020_PQ_EOTF
metalLayer.colorspace = CGColorSpace(name: name)
```

```
CAMetalLayer *metalLayer = [CAMetalLayer new];
metalLayer.wantsExtendedDynamicRangeContent = YES;
metalLayer.pixelFormat = MTLPixelFormatBGR10A2Unorm;
const CFStringRef name = kCGColorSpaceITUR_2020_PQ_EOTF;
CGColorSpaceRef colorspace = CGColorSpaceCreateWithName(name);
metalLayer.colorspace = colorspace;
CGColorSpaceRelease(colorspace);
```

## See Also

### High Dynamic Range Content

Processing HDR Images with Metal

Implement a post-processing pipeline using the latest features on Apple GPUs.

Displaying HDR Content in a Metal Layer

Bring your high dynamic range (HDR) content to compatible Mac displays.

Determining Support for EDR Values

Check whether a display supports EDR.

Using System Tone Mapping on Video Content

Use EDR metadata to apply the default system tone mapping to a layer.

Performing Your Own Tone Mapping

Apply your own tone mapping to get the exact behavior you want.

Implementing Tone Mapping on Reference Displays

Detect reference displays and keep your content within the capabilities of the display hardware.

