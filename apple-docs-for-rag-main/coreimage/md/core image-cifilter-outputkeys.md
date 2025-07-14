

- Core Image
- CIFilter
-  outputKeys 

Instance Property

# outputKeys

The names of all output parameters from the filter.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
var outputKeys: [String] { get }
```

## See Also

### Getting Filter Parameters and Attributes

var name: String

A name associated with a filter.

var isEnabled: Bool

A Boolean value that determines whether the filter is enabled. Animatable.

var attributes: [String : Any]

A dictionary of key-value pairs that describe the filter.

var inputKeys: [String]

The names of all input parameters to the filter.

var outputImage: CIImage?

Returns a CIImage object that encapsulates the operations configured in the filter.

