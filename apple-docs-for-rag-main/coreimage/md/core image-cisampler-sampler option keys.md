

- Core Image
- CISampler
-  Sampler Option Keys 

API Collection

# Sampler Option Keys

Keys for creating a sampler.

## Topics

### Constants

let kCISamplerAffineMatrix: String

The key for an affine matrix. The associated value is an `NSArray` object (\[*a b c d tx ty*\]) that defines the transformation to apply to the sampler.

let kCISamplerWrapMode: String

The key for the sampler wrap mode. The wrap mode specifies how Core Image produces pixels that are outside the extent of the sample. Possible values are kCISamplerWrapBlack and kCISamplerWrapClamp.

let kCISamplerFilterMode: String

The key for the filtering to use when sampling the image. Possible values are kCISamplerFilterNearest and kCISamplerFilterLinear.

let kCISamplerColorSpace: String

The key for the color space to use when sampling the image. The associated value must be an RGB CGColorSpace object. Using this option specifies that samples should be converted to this color space before being passed to a kernel. If not specified, samples will be passed to the kernel in the working color space of the Core Image context used to render the image.

