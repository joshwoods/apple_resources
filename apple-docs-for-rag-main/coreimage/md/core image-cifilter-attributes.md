

- Core Image
- CIFilter
-  attributes 

Instance Property

# attributes

A dictionary of key-value pairs that describe the filter.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
var attributes: [String : Any] { get }
```

## Discussion

This dictionary contains two kinds of key-value pairs:

- Keys listed in Filter Attribute Keys describe the filter, providing information such as a human-readable name and categories you can use to organize filters in your app’s UI.

- Other keys, including those listed in Filter Parameter Keys and those starting with “input” or “output”, describe parameters that control the filter’s behavior. For each parameter key, the corresponding value is another dictionary describing possible values for that parameter, such as the value class and minimum/maximum values. You can use this information to build a UI to control the filter.

For example, the attributes dictionary for the `CIColorControls` filter contains the following information:

CIColorControls:
{
    CIAttributeFilterCategories = (
        CICategoryColorAdjustment,
        CICategoryVideo,
        CICategoryStillImage,
        CICategoryInterlaced,
        CICategoryNonSquarePixels,
        CICategoryBuiltIn
    );
    CIAttributeFilterDisplayName = &quot;Color Controls&quot;;
    CIAttributeFilterName = CIColorControls;
    inputBrightness = {
        CIAttributeClass = NSNumber;
        CIAttributeDefault = 0;
        CIAttributeIdentity = 0;
        CIAttributeMin = -1;
        CIAttributeSliderMax = 1;
        CIAttributeSliderMin = -1;
        CIAttributeType = CIAttributeTypeScalar;
    };
    inputContrast = {
        CIAttributeClass = NSNumber;
        CIAttributeDefault = 1;
        CIAttributeIdentity = 1;
        CIAttributeMin = 0.25;
        CIAttributeSliderMax = 4;
        CIAttributeSliderMin = 0.25;
        CIAttributeType = CIAttributeTypeScalar;
    };
    inputImage = {CIAttributeClass = CIImage; };
    inputSaturation = {
        CIAttributeClass = NSNumber;
        CIAttributeDefault = 1;
        CIAttributeIdentity = 1;
        CIAttributeMin = 0;
        CIAttributeSliderMax = 3;
        CIAttributeSliderMin = 0;
        CIAttributeType = CIAttributeTypeScalar;
    };
    outputImage = {CIAttributeClass = CIImage; };
}

## See Also

### Getting Filter Parameters and Attributes

var name: String

A name associated with a filter.

var isEnabled: Bool

A Boolean value that determines whether the filter is enabled. Animatable.

var inputKeys: [String]

The names of all input parameters to the filter.

var outputKeys: [String]

The names of all output parameters from the filter.

var outputImage: CIImage?

Returns a CIImage object that encapsulates the operations configured in the filter.

