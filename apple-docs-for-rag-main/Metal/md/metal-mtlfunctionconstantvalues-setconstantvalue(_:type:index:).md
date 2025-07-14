

- Metal
- MTLFunctionConstantValues
-  setConstantValue(\_:type:index:) 

Instance Method

# setConstantValue(\_:type:index:)

Sets a value for a function constant at a specific index.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func setConstantValue(
    _ value: UnsafeRawPointer,
    type: MTLDataType,
    index: Int
)
```

## Parameters 

`value`  

A pointer to the constant value.

`type`  

The data type of the function constant.

`index`  

The index of the function constant.

## Discussion

Declare a single function constant in Metal Shading Language (MSL).

```
constant bool a [[ function_constant(0) ]];
```

Set its value by assigning with a specific index.

- Swift
- Objective-C

```
var a = true
let constantValues = MTLFunctionConstantValues()
constantValues.setConstantValue(&a, type: .bool, at: 0)
```

```
const bool a = true;
MTLFunctionConstantValues* constantValues = [MTLFunctionConstantValues new];
[constantValues setConstantValue:&a type:MTLDataTypeBool atIndex:0];
```

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Setting Constant Values

func setConstantValue(UnsafeRawPointer, type: MTLDataType, withName: String)

Sets a value for a function constant with a specific name.

func setConstantValues(UnsafeRawPointer, type: MTLDataType, range: Range&lt;Int>)

Sets values for a group of function constants within a specific index range.

