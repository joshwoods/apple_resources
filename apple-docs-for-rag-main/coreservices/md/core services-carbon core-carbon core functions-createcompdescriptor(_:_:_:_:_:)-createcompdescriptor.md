

- Core Services
- Carbon Core
- Carbon Core Functions
-  CreateCompDescriptor(\_:\_:\_:\_:\_:) 

Function

# CreateCompDescriptor(\_:\_:\_:\_:\_:)

Creates a comparison descriptor that specifies how to compare one or more Apple event objects with either another Apple event object or a descriptor.

macOS 10.0+

``` source
func CreateCompDescriptor(
    _ comparisonOperator: DescType,
    _ operand1: UnsafeMutablePointer!,
    _ operand2: UnsafeMutablePointer!,
    _ disposeInputs: Bool,
    _ theDescriptor: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`comparisonOperator`  

The comparison operator for comparing the descriptors in the `operand1` and `operand2` parameters. The standard comparison operators are defined in Comparison Operator Constants.

The actual comparison of the two operands is performed by the object comparison function provided by the client application. The way a comparison operator is interpreted is up to each application.

See DescType.

`operand1`  

A pointer to an object specifier. See AEDesc.

`operand2`  

A pointer to a descriptor (which can be an object specifier or any other descriptor) whose value is compared to the value of `operand1`. See AEDesc.

`disposeInputs`  

A Boolean value. Pass `TRUE` if the function should automatically dispose of any descriptors you have provided in the `operand1` and `operand2` parameters to the function. Pass `FALSE` if your application will dispose of the descriptors itself. A value of `FALSE` may be more efficient for some applications because it allows them to reuse descriptors.

`theDescriptor`  

A pointer to a descriptor. On successful return, the comparison descriptor created by `CreateCompDescriptor`. Your application must dispose of this descriptor after it has finished using it. See AEDesc.

## Return Value

A result code. See Result Codes.

## See Also

### Creating Object Specifiers

func CreateLogicalDescriptor(UnsafeMutablePointer&lt;AEDescList>!, DescType, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a logical descriptor that specifies a logical operator and one or more logical terms for the Apple Event Manager to evaluate.

func CreateObjSpecifier(DescType, UnsafeMutablePointer&lt;AEDesc>!, DescType, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Assembles an object specifier that identifies one or more Apple event objects, from other descriptors.

func CreateOffsetDescriptor(Int, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates an offset descriptor that specifies the position of an element in relation to the beginning or end of its container.

func CreateRangeDescriptor(UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a range descriptor that specifies a series of consecutive elements in the same container.

