

- Core Services
- Carbon Core
- Carbon Core Functions
-  CreateRangeDescriptor(\_:\_:\_:\_:) 

Function

# CreateRangeDescriptor(\_:\_:\_:\_:)

Creates a range descriptor that specifies a series of consecutive elements in the same container.

Mac Catalyst 13.1+macOS 10.0+

``` source
func CreateRangeDescriptor(
    _ rangeStart: UnsafeMutablePointer!,
    _ rangeStop: UnsafeMutablePointer!,
    _ disposeInputs: Bool,
    _ theDescriptor: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`rangeStart`  

A pointer to an object specifier that identifies the first Apple event object in the range. See AEDesc.

`rangeStop`  

A pointer to an object specifier that identifies the last Apple event object in the range. See AEDesc.

`disposeInputs`  

A Boolean value. Pass (`TRUE`) if the function should dispose of the descriptors for the `rangeStart` and `rangeStop` parameters and set them to the null descriptor or (`FALSE`) if your application will. A value of `FALSE` may be more efficient for some applications because it allows them to reuse descriptors.

`theDescriptor`  

A pointer to a descriptor. On successful return, the range descriptor created by `CreateRangeDescriptor`. Your application must dispose of this descriptor after it has finished using it. See AEDesc.

## Return Value

A result code. See Result Codes.

## Discussion

Although the `rangeStart` and `rangeStop` parameters can be any object specifiers—including object specifiers that specify more than one Apple event object—most applications expect these parameters to specify single Apple event objects.

## See Also

### Creating Object Specifiers

func CreateCompDescriptor(DescType, UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a comparison descriptor that specifies how to compare one or more Apple event objects with either another Apple event object or a descriptor.

func CreateLogicalDescriptor(UnsafeMutablePointer&lt;AEDescList>!, DescType, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a logical descriptor that specifies a logical operator and one or more logical terms for the Apple Event Manager to evaluate.

func CreateObjSpecifier(DescType, UnsafeMutablePointer&lt;AEDesc>!, DescType, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Assembles an object specifier that identifies one or more Apple event objects, from other descriptors.

func CreateOffsetDescriptor(Int, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates an offset descriptor that specifies the position of an element in relation to the beginning or end of its container.

