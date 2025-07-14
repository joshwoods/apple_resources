

- Core Image
- CIFilter
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that determines whether the filter is enabled. Animatable.

macOS 10.5+

``` source
var isEnabled: Bool { get set }
```

## Discussion

The filter is applied to its input when this property is set to `true` (the default).

Use this property in conjunction with the name property when attaching filters to Core Animation layers and accessing or animating filter properties through key-value animations. Core Animation can animate this property on a layer.

## See Also

### Getting Filter Parameters and Attributes

var name: String

A name associated with a filter.

var attributes: [String : Any]

A dictionary of key-value pairs that describe the filter.

var inputKeys: [String]

The names of all input parameters to the filter.

var outputKeys: [String]

The names of all output parameters from the filter.

var outputImage: CIImage?

Returns a CIImage object that encapsulates the operations configured in the filter.

