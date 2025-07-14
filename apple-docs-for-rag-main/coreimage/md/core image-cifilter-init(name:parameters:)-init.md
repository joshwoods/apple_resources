

- Core Image
- CIFilter
-  init(name:parameters:) 

Initializer

# init(name:parameters:)

Creates a `CIFilter` object for a specific kind of filter and initializes the input values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
init?(
    name: String,
    parameters params: [String : Any]?
)
```

## Parameters 

`name`  

The name of the filter. You must make sure the name is spelled correctly, otherwise your app will run but not produce any output images. For that reason, you should check for the existence of the filter after calling this method.

`params`  

A list of key-value pairs to set as input values to the filter. Each key is a constant that specifies the name of an input parameter for the filter, and the corresponding value is the value for that parameter. See Core Image Filter Reference for built-in filters and their allowed parameters.

## Return Value

A `CIFilter` object whose input values are initialized.

## Discussion

Use this method to quickly create and configure a `CIFilter` instance, as in the example below.

CIFilter *f = [CIFilter filterWithName: @&quot;CIColorControls&quot;
                   withInputParameters: @{
                             @&quot;inputImage&quot;      : inImage,
                             @&quot;inputSaturation&quot; : @0.5,
                             @&quot;inputBrightness&quot; : @1.2,
                             @&quot;inputContrast&quot;   : @1.3
                                         }];

## See Also

### Creating a Filter

init?(name: String)

Creates a `CIFilter` object for a specific kind of filter.

