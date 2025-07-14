

- Core Image
-  CIFilter 

Class

# CIFilter

An image processor that produces an image by manipulating one or more input images or by generating new image data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
class CIFilter : NSObject
```

## Overview

The `CIFilter` class produces a CIImage object as output. Typically, a filter takes one or more images as input. Some filters, however, generate an image based on other types of input parameters. The parameters of a `CIFilter` object are set and retrieved through the use of key-value pairs.

You use the `CIFilter` object in conjunction with other Core Image classes, such as CIImage, CIContext, and CIColor, to take advantage of the built-in Core Image filters when processing images, creating filter generators, or writing custom filters.

`CIFilter` objects are mutable, and thus cannot be shared safely among threads. Each thread must create its own `CIFilter` objects, but you can pass a filter’s immutable input and output `CIImage` objects between threads.

To get a quick overview of how to set up and use Core Image filters, see Core Image Programming Guide.

### Create Type-Safe Filters

Core Image provides methods that create type-safe CIFilter instances. Use these filters to avoid run-time errors that can occur when relying on Core Image’s string-based API.

To use the type-safe API, import `CoreImage.CIFilterBuiltins`:

import CoreImage
import CoreImage.CIFilterBuiltins

The type-safe approach returns a non-optional filter. Because the returned filter conforms to the relevant protocol—for example, CIFalseColor in the case of falseColor()—the parameters are available as properties. The following creates and applies a false color filter:

func falseColor(inputImage: CIImage) -> CIImage? {
    let falseColorFilter = CIFilter.falseColor()
    falseColorFilter.color0 = CIColor(red: 1, green: 1, blue: 0)
    falseColorFilter.color1 = CIColor(red: 0, green: 0, blue: 1)
    falseColorFilter.inputImage = inputImage
    return falseColorFilter.outputImage
}

The false color filter maps luminance to a color ramp of two colors:

### Subclassing Notes

You can subclass `CIFilter` in order to create custom filter effects:

- By chaining together two or more built-in Core Image filters

- By using an image-processing kernel that you write

Regardless of whether your subclass provides its effect by chaining filters or implementing its own kernel, you should:

- Declare any input parameters as properties whose names are prefixed with `input`, such as `inputImage`.

- Override the setDefaults() methods to provide default values for any input parameters you’ve declared.

- Implement an `outputImage` method to create a new CIImage with your filter’s effect.

The `CIFilter` class automatically manages input parameters when archiving, copying, and deallocating filters. For this reason, your subclass must obey the following guidelines to ensure proper behavior:

- Store input parameters in instance variables whose names are prefixed with `input`.

  Don’t use auto-synthesized instance variables, because their names are automatically prefixed with an underscore. Instead, synthesize the property manually. For example:

  `@synthesize inputMyParameter;`

- If using manual reference counting, don’t release input parameter instance variables in your `dealloc` method implementation. The `dealloc` implementation in the `CIFilter` class uses Key-value coding to automatically set the values of all input parameters to `nil`.

## Topics

### Creating a Filter

init?(name: String)

Creates a `CIFilter` object for a specific kind of filter.

init?(name: String, parameters: [String : Any]?)

Creates a `CIFilter` object for a specific kind of filter and initializes the input values.

### Configuring Type-Safe Filters

Configure Core Image filters that expose their attributes as properties.

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

Halftone Effect Filters

Reduction Filters

Sharpening Filters

Stylizing Filters

Tile Effect Filters

Transition Filters

### Accessing Registered Filters

class func filterNames(inCategories: [String]?) -> [String]

Returns an array of all published filter names that match all the specified categories.

class func filterNames(inCategory: String?) -> [String]

Returns an array of all published filter names in the specified category.

### Registering a Filter

class func registerName(String, constructor: any CIFilterConstructor, classAttributes: [String : Any])

Publishes a custom filter that is not packaged as an image unit.

### Getting Filter Parameters and Attributes

var name: String

A name associated with a filter.

var isEnabled: Bool

A Boolean value that determines whether the filter is enabled. Animatable.

var attributes: [String : Any]

A dictionary of key-value pairs that describe the filter.

var inputKeys: [String]

The names of all input parameters to the filter.

var outputKeys: [String]

The names of all output parameters from the filter.

var outputImage: CIImage?

Returns a CIImage object that encapsulates the operations configured in the filter.

### Setting Default Values

func setDefaults()

Sets all input values for a filter to default values.

### Applying a Filter

func apply(CIKernel, arguments: [Any]?, options: [String : Any]?) -> CIImage?

Produces a CIImage object by applying arguments to a kernel function and using options to control how the kernel function is evaluated.

### Getting Localized Information for Registered Filters

class func localizedName(forFilterName: String) -> String?

Returns the localized name for the specified filter name.

class func localizedName(forCategory: String) -> String

Returns the localized name for the specified filter category.

class func localizedDescription(forFilterName: String) -> String?

Returns the localized description of a filter for display in the user interface.

class func localizedReferenceDocumentation(forFilterName: String) -> URL?

Returns the location of the localized reference documentation that describes the filter.

### Creating a Configuration View for a Filter

func view(forUIConfiguration: [AnyHashable : Any]!, excludedKeys: [Any]!) -> IKFilterUIView!

Returns a filter view for the filter.

### Constants

Filter Attribute Keys

Attributes for a filter and its parameters.

Data Type Attributes

Numeric data types.

Vector Quantity Attributes

Vector data types.

Color Attribute Keys

Color types.

Image Attribute Keys

Image Types

Filter Category Keys

Categories of filters.

Options for Applying a Filter

Options that control the application of a custom Core Image filter.

User Interface Control Options

Sets of controls for various user scenarios.

User Interface Options

Keys or values for the size of the input parameter controls for a filter view.

Filter Parameter Keys

Keys for input parameters to filters.

RAW Image Options

Options for creating a `CIFilter` object from RAW image data.

### Deprecated

init!(cvPixelBuffer: CVPixelBuffer!, properties: [AnyHashable : Any]!, options: [CIRAWFilterOption : Any]!)

Creates a filter from a Core Video pixel buffer.

Deprecated

init!(imageData: Data!, options: [CIRAWFilterOption : Any]!)

Creates a filter that allows the processing of RAW images.

Deprecated

init!(imageURL: URL!, options: [CIRAWFilterOption : Any]!)

Creates a filter that allows the processing of RAW images.

Deprecated

struct CIRAWFilterOptionDeprecated

class func serializedXMP(from: [CIFilter], inputImageExtent: CGRect) -> Data?

Serializes filter parameters into XMP form that is suitable for embedding in an image.

Deprecated

class func filterArray(fromSerializedXMP: Data, inputImageExtent: CGRect, error: NSErrorPointer) -> [CIFilter]

Returns an array of filter objects de-serialized from XMP data.

Deprecated

class func supportedRawCameraModels() -> [String]!Deprecated

### Type Methods

class func areaAlphaWeightedHistogram() -> any CIFilter &amp; CIAreaHistogram

class func areaBoundsRed() -> any CIFilter &amp; CIAreaBoundsRed

class func maximumScaleTransform() -> any CIFilter &amp; CIMaximumScaleTransform

class func toneMapHeadroom() -> any CIFilter &amp; CIToneMapHeadroom

## Relationships

### Inherits From

- NSObject

### Conforms To

- NSCopying
- NSSecureCoding

## See Also

### Filters

class CIRAWFilter

A filter subclass that produces an image by manipulating RAW image sensor data from a digital camera or scanner.

class CIColor

The component values defining a color in a specific color space.

class CIVector

A container for coordinate values, direction vectors, matrices, and other non-scalar values, typically used in Core Image for filter parameters.

