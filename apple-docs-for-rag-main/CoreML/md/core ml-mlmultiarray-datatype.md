

- Core ML
- MLMultiArray
-  dataType 

Instance Property

# dataType

The underlying type of the multiarray.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var dataType: MLMultiArrayDataType { get }
```

## See Also

### Inspecting a Multiarray

var count: Int

The total number of elements in the multiarray.

var shape: [NSNumber]

The multiarray’s multidimensional shape as a number array in which each element’s value is the size of the corresponding dimension.

var strides: [NSNumber]

A number array in which each element is the number of memory locations that span the length of the corresponding dimension.

