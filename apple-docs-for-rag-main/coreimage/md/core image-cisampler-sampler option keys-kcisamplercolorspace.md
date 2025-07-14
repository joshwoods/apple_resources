

- Core Image
- CISampler
- Sampler Option Keys
-  kCISamplerColorSpace 

Global Variable

# kCISamplerColorSpace

The key for the color space to use when sampling the image. The associated value must be an RGB CGColorSpace object. Using this option specifies that samples should be converted to this color space before being passed to a kernel. If not specified, samples will be passed to the kernel in the working color space of the Core Image context used to render the image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
let kCISamplerColorSpace: String
```

