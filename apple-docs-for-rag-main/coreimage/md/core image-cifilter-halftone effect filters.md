

- Core Image
- CIFilter
-  Halftone Effect Filters 

API Collection

# Halftone Effect Filters

## Topics

### Filters

class func circularScreen() -> any CIFilter &amp; CICircularScreen

Adds a circular overlay to an image.

class func cmykHalftone() -> any CIFilter &amp; CICMYKHalftone

Adds a series of colorful dots to an image.

class func dotScreen() -> any CIFilter &amp; CIDotScreen

Creates a monochrome image with a series of dots to add detail.

class func hatchedScreen() -> any CIFilter &amp; CIHatchedScreen

Creates a monochrome image with a series of lines to add detail.

class func lineScreen() -> any CIFilter &amp; CILineScreen

Creates a monochrome image with a series of small lines to add detail.

### Protocols

protocol CICircularScreen

The properties you use to configure a circular screen filter.

protocol CICMYKHalftone

The properties you use to configure a CMYK halftone filter.

protocol CIDotScreen

The properties you use to configure a dot screen filter.

protocol CIHatchedScreen

The properties you use to configure a hatched screen filter.

protocol CILineScreen

The properties you use to configure a line screen filter.

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

Gradient Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

Transition Filters

