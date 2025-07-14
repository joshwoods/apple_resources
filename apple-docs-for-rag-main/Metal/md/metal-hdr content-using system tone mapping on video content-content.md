

- Metal
- HDR Content
-  Using System Tone Mapping on Video Content 

Article

# Using System Tone Mapping on Video Content

Use EDR metadata to apply the default system tone mapping to a layer.

## Overview

When processing video content, you usually want to work in a linear color space. You also want to display content that’s consistent with how playback would appear in AVFoundation or other playback mechanisms. To create content in your app that is consistent with the system behavior, create a Metal layer with a linear color space and attach an CAEDRMetadata object defining how the system should tone map the video content.

The code below creates a Metal layer with an extended linear BT.2020 color space and metadata that applies an HDR10 tone mapping based on the reference display.

- Swift
- Objective-C

```
let metalLayer = CAMetalLayer()
metalLayer.wantsExtendedDynamicRangeContent = true
metalLayer.pixelFormat = .rgba16Float

let name = CGColorSpace.extendedLinearITUR_2020
metalLayer.colorspace = CGColorSpace(name: name)

let edrMetadata = CAEDRMetadata(minLuminance: 0.5, maxLuminance: 1000, opticalOutputScale: 100)
metalLayer.edrMetadata = edrMetadata
```

```
CAMetalLayer *metalLayer = [CAMetalLayer new];
metalLayer.wantsExtendedDynamicRangeContent = YES;
metalLayer.pixelFormat = MTLPixelFormatRGBA16Float;

const CFStringRef name = kCGColorSpaceExtendedLinearITUR_2020;
CGColorSpaceRef colorspace = CGColorSpaceCreateWithName(name);
metalLayer.colorspace = colorspace;

CGColorSpaceRelease(colorspace);
CAEDRMetadata *edrMetaData = [CAEDRMetadata HDR10MetadataWithMinLuminance: 0.005 maxLuminance: 1000 opticalOutputScale: 100];
metalLayer.EDRMetadata = edrMetaData;
```

Your rendering code needs to generate pixel values consistent with the EDR metadata object. For example, in the above code, the `opticalOutputScale` was set to `100`, so a pixel value of `1.0` corresponds to `100` nits. For more information, see CAEDRMetadata.

## See Also

### High Dynamic Range Content

Processing HDR Images with Metal

Implement a post-processing pipeline using the latest features on Apple GPUs.

Displaying HDR Content in a Metal Layer

Bring your high dynamic range (HDR) content to compatible Mac displays.

Determining Support for EDR Values

Check whether a display supports EDR.

Using Color Spaces to Display HDR Content

Use a color space when you don’t need to edit or process the pixel data.

Performing Your Own Tone Mapping

Apply your own tone mapping to get the exact behavior you want.

Implementing Tone Mapping on Reference Displays

Detect reference displays and keep your content within the capabilities of the display hardware.

