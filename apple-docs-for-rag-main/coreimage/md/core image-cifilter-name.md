

- Core Image
- CIFilter
-  name 

Instance Property

# name

A name associated with a filter.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 10.0+visionOS 1.0+

``` source
var name: String { get set }
```

## Discussion

You use a filter’s name to construct key paths to its attributes when the filter is attached to a Core Animation layer. For example, if a CALayer object has an attached `CIFilter` instance whose name is `myExposureFilter`, you can refer to attributes of the filter using a key path such as `filters.myExposureFilter.inputEV`. Layer animations may also access filter attributes via these key paths.

Core Animation can animate this property on a layer.

The default value for this property is `nil`.

## See Also

### Getting Filter Parameters and Attributes

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

