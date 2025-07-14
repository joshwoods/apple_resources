

- Metal
-  MTLFunctionConstantValues 

Class

# MTLFunctionConstantValues

A set of constant values that specialize a graphics or compute function.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class MTLFunctionConstantValues
```

## Overview

A MTLFunctionConstantValues object sets constant values for function constants. Function constants are declared with the `[[ function_constant(index) ]]` attribute in Metal shading language source code. Refer to the Metal Shading Language Guide for more information.

Single constant values can be set individually by index or name. Multiple constant values can be set together with an index range.

A single MTLFunctionConstantValues object can be applied to multiple MTLFunction objects (for example, a vertex function and a fragment function). After a specialized function has been created, any changes to its constant values have no further effect on it. However, you can reset, add, or modify any constant values in the MTLFunctionConstantValues object and reuse it to create another MTLFunction object.

## Topics

### Setting Constant Values

func setConstantValue(UnsafeRawPointer, type: MTLDataType, index: Int)

Sets a value for a function constant at a specific index.

func setConstantValue(UnsafeRawPointer, type: MTLDataType, withName: String)

Sets a value for a function constant with a specific name.

func setConstantValues(UnsafeRawPointer, type: MTLDataType, range: Range&lt;Int>)

Sets values for a group of function constants within a specific index range.

### Resetting Constant Values

func reset()

Deletes all previously set constant values.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Compile-Time Variant Functions

class MTLFunctionConstant

A constant that specializes the behavior of a shader.

