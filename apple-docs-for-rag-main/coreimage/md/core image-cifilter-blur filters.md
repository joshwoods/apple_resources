

- Core Image
- CIFilter
-  Blur Filters 

API Collection

# Blur Filters

## Topics

### Filters

class func bokehBlur() -> any CIFilter &amp; CIBokehBlur

Applies a bokeh effect to an image.

class func boxBlur() -> any CIFilter &amp; CIBoxBlur

Applies a square-shaped blur to an area of an image.

class func discBlur() -> any CIFilter &amp; CIDiscBlur

Applies a circle-shaped blur to an area of an image.

class func gaussianBlur() -> any CIFilter &amp; CIGaussianBlur

Blurs an image with a Gaussian distribution pattern.

class func maskedVariableBlur() -> any CIFilter &amp; CIMaskedVariableBlur

Blurs a specified portion of an image.

class func median() -> any CIFilter &amp; CIMedian

Calculates the median of an image to refine detail.

class func morphologyGradient() -> any CIFilter &amp; CIMorphologyGradient

Detects and highlights edges of objects.

class func morphologyMaximum() -> any CIFilter &amp; CIMorphologyMaximum

Blurs a circular area by enlarging contrasting pixels.

class func morphologyMinimum() -> any CIFilter &amp; CIMorphologyMinimum

Blurs a circular area by reducing contrasting pixels.

class func morphologyRectangleMaximum() -> any CIFilter &amp; CIMorphologyRectangleMaximum

Blurs a rectangular area by enlarging contrasting pixels.

class func morphologyRectangleMinimum() -> any CIFilter &amp; CIMorphologyRectangleMinimum

Blurs a rectangular area by reducing contrasting pixels.

class func motionBlur() -> any CIFilter &amp; CIMotionBlur

Creates motion blur on an image.

class func noiseReduction() -> any CIFilter &amp; CINoiseReduction

Reduces noise by sharpening the edges of objects.

class func zoomBlur() -> any CIFilter &amp; CIZoomBlur

Creates a zoom blur centered around a single point on the image.

### Protocols

protocol CIBokehBlur

The properties you use to configure a bokeh blur filter.

protocol CIBoxBlur

The properties you use to configure a box blur filter.

protocol CIDiscBlur

The properties you use to configure a disc blur filter.

protocol CIGaussianBlur

The properties you use to configure a Gaussian blur filter.

protocol CIMaskedVariableBlur

The properties you use to configure a masked variable blur filter.

protocol CIMedian

The properties you use to configure a median filter.

protocol CIMorphologyGradient

The properties you use to configure a morphology gradient filter.

protocol CIMorphologyMaximum

The properties you use to configure a morphology maximum filter.

protocol CIMorphologyMinimum

The properties you use to configure a morphology minimum filter.

protocol CIMorphologyRectangleMaximum

The properties you use to configure a morphology rectangle maximum filter.

protocol CIMorphologyRectangleMinimum

The properties you use to configure a morphology rectangle minimum filter.

protocol CIMotionBlur

The properties you use to configure a motion blur filter.

protocol CINoiseReduction

The properties you use to configure a noise reduction filter.

protocol CIZoomBlur

The properties you use to configure a zoom blur filter.

## See Also

### Configuring Type-Safe Filters

protocol CIFilterProtocol

The properties you use to configure a Core Image filter.

Color Adjustment Filters

Color Effect Filters

Composite Operations

Convolution Filters

Distortion Filters

Generator Filters

Geometry Adjustment Filters

Gradient Filters

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

Transition Filters

