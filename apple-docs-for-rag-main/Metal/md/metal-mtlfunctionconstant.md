

- Metal
-  MTLFunctionConstant 

Class

# MTLFunctionConstant

A constant that specializes the behavior of a shader.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class MTLFunctionConstant
```

## Overview

Don’t create a MTLFunctionConstant object directly. Instead, the list of function constants for a function by querying the `functionConstants` property of a MTLFunction object.

A MTLFunctionConstant object should only be obtained from a nonspecialized function created with the makeFunction(name:) method. You only need a MTLFunctionConstant object if you don’t have sufficient information to create a MTLFunctionConstantValues object used to create a specialized function with the makeFunction(name:constantValues:) or makeFunction(name:constantValues:completionHandler:) method.

## Topics

### Reading the Function Constant’s Properties

var name: String

The name of the function constant.

var type: MTLDataType

The data type of the function constant.

var index: Int

The index of the function constant.

var required: Bool

A Boolean value indicating whether the function constant must be provided to specialize the function.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Compile-Time Variant Functions

class MTLFunctionConstantValues

A set of constant values that specialize a graphics or compute function.

