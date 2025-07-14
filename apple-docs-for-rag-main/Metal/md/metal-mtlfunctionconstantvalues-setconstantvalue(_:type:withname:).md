

- Metal
- MTLFunctionConstantValues
-  setConstantValue(\_:type:withName:) 

Instance Method

# setConstantValue(\_:type:withName:)

Sets a value for a function constant with a specific name.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func setConstantValue(
    _ value: UnsafeRawPointer,
    type: MTLDataType,
    withName name: String
)
```

## Parameters 

`value`  

A pointer to the constant value.

`type`  

The data type of the function constant.

`name`  

The name of the function constant.

## Discussion

The first example declares a single function constant in a Metal Shading Language file.

```
constant bool a [[ function_constant(0) ]];
```

The next example sets that Boolean value by providing its specific name.

- Swift
- Objective-C

```
var a = true
let constantValues = MTLFunctionConstantValues()
constantValues.setConstantValue(&a, type: .bool, withName: "a")
```

```
const bool a = true;
MTLFunctionConstantValues* constantValues = [MTLFunctionConstantValues new];
[constantValues setConstantValue:&a type:MTLDataTypeBool withName:@"a"];
```

## See Also

### Setting Constant Values

func setConstantValue(UnsafeRawPointer, type: MTLDataType, index: Int)

Sets a value for a function constant at a specific index.

func setConstantValues(UnsafeRawPointer, type: MTLDataType, range: Range&lt;Int>)

Sets values for a group of function constants within a specific index range.

