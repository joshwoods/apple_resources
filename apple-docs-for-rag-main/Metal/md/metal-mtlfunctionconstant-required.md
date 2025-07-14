

- Metal
- MTLFunctionConstant
-  required 

Instance Property

# required

A Boolean value indicating whether the function constant must be provided to specialize the function.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var required: Bool { get }
```

## Discussion

This value is true if a constant value must be provided for the function constant. A function constant is optional only if it is referenced in a call to the built-in `is_function_constant_defined(name)` function.

Refer to the Metal Shading Language Guide for more information.

## See Also

### Reading the Function Constant’s Properties

var name: String

The name of the function constant.

var type: MTLDataType

The data type of the function constant.

var index: Int

The index of the function constant.

