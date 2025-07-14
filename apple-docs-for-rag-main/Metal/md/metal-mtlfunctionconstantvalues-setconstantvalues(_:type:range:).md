

- Metal
- MTLFunctionConstantValues
-  setConstantValues(\_:type:range:) 

Instance Method

# setConstantValues(\_:type:range:)

Sets values for a group of function constants within a specific index range.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOS

``` source
func setConstantValues(
    _ values: UnsafeRawPointer,
    type: MTLDataType,
    range: Range
)
```

## Parameters 

`values`  

A pointer to the constant values.

`type`  

The data type of the function constants.

`range`  

The range of the function constant indices.

## Discussion

Declare multiple function constants in Metal Shading Language (MSL).

```
constant bool a [[ function_constant(0) ]];
constant bool b [[ function_constant(1) ]];
constant bool c [[ function_constant(2) ]];
```

Set their values by assigning an index range of an array.

```
let abc = [true, true, true]
let constantValues = MTLFunctionConstantValues()
constantValues.setConstantValues(abc,
                                 type: .bool,
                                 with: NSMakeRange(0, 3))
```

## See Also

### Setting Constant Values

func setConstantValue(UnsafeRawPointer, type: MTLDataType, index: Int)

Sets a value for a function constant at a specific index.

func setConstantValue(UnsafeRawPointer, type: MTLDataType, withName: String)

Sets a value for a function constant with a specific name.

