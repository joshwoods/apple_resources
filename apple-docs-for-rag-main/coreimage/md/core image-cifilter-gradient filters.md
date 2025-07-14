

- Core Image
- CIFilter
-  Gradient Filters 

API Collection

# Gradient Filters

## Topics

### Filters

class func gaussianGradient() -> any CIFilter &amp; CIGaussianGradient

Generates a gradient that varies from one color to another using a Gaussian distribution.

class func hueSaturationValueGradient() -> any CIFilter &amp; CIHueSaturationValueGradient

Generates a gradient representing a specified color space.

class func linearGradient() -> any CIFilter &amp; CILinearGradient

Generates a color gradient that varies along a linear axis between two defined endpoints.

class func radialGradient() -> any CIFilter &amp; CIRadialGradient

Generates a gradient that varies radially between two circles having the same center.

class func smoothLinearGradient() -> any CIFilter &amp; CISmoothLinearGradient

Generates a gradient that blends colors along a linear axis between two defined endpoints.

### Protocols

protocol CIGaussianGradient

The properties you use to configure a Gaussian gradient filter.

protocol CIHueSaturationValueGradient

The properties you use to configure a hue-saturation-value gradient filter.

protocol CILinearGradient

The properties you use to configure a linear gradient filter.

protocol CIRadialGradient

The properties you use to configure a radial gradient filter.

protocol CISmoothLinearGradient

The properties you use to configure a smooth linear gradient filter.

## See Also

### Configuring Type-Safe Filters

protocol CIFilterProtocol

The properties you use to configure a Core Image filter.

Blur Filters

Color Adjustment Filters

Color Effect Filters

Composite Operations

Convolution Filters

Distortion Filters

Generator Filters

Geometry Adjustment Filters

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

Transition Filters

