

- Core Services
- Carbon Core
- Carbon Core Functions
-  CreateLogicalDescriptor(\_:\_:\_:\_:) 

Function

# CreateLogicalDescriptor(\_:\_:\_:\_:)

Creates a logical descriptor that specifies a logical operator and one or more logical terms for the Apple Event Manager to evaluate.

macOS 10.0+

``` source
func CreateLogicalDescriptor(
    _ theLogicalTerms: UnsafeMutablePointer!,
    _ theLogicOperator: DescType,
    _ disposeInputs: Bool,
    _ theDescriptor: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theLogicalTerms`  

A pointer to a list containing comparison descriptors (`typeLogicalDescriptor`), logical descriptors (`typeCompDescriptor`), or both. If the value of the parameter `theLogicOperator` is `kAEAND` or `kAEOR`, the list can contain any number of descriptors. If the value of the parameter `theLogicOperator` is `kAENOT`, logically this list should contain a single descriptor. However, the function will not return an error if the list contains more than one descriptor for a logical operator of `kAENOT`. See AEDescList.

`theLogicOperator`  

A logical operator represented by one of the constants described in Constants for Object Specifiers, Positions, and Logical and Comparison Operations. What you pass for this parameter helps determine what you pass for the `theLogicalTerms` parameter. See DescType.

`disposeInputs`  

A Boolean value. Pass `TRUE` if the function should automatically dispose of the descriptors you have provided in the `theLogicalTerms` parameter or (`FALSE`) if your application will. A value of `FALSE` may be more efficient for some applications because it allows them to reuse descriptors.

`theDescriptor`  

A pointer to a descriptor. On successful return, the logical descriptor created by `CreateLogicalDescriptor`. Your application must dispose of this descriptor after it has finished using it. See AEDesc.

## Return Value

A result code. See Result Codes.

## Discussion

The `CreateLogicalDescriptor` function creates a logical descriptor, which specifies a logical operator and one or more logical terms for the Apple Event Manager to evaluate.

## See Also

### Creating Object Specifiers

func CreateCompDescriptor(DescType, UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a comparison descriptor that specifies how to compare one or more Apple event objects with either another Apple event object or a descriptor.

func CreateObjSpecifier(DescType, UnsafeMutablePointer&lt;AEDesc>!, DescType, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Assembles an object specifier that identifies one or more Apple event objects, from other descriptors.

func CreateOffsetDescriptor(Int, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates an offset descriptor that specifies the position of an element in relation to the beginning or end of its container.

func CreateRangeDescriptor(UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a range descriptor that specifies a series of consecutive elements in the same container.

