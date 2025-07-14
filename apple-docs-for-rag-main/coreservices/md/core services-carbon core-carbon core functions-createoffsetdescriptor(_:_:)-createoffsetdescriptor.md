

- Core Services
- Carbon Core
- Carbon Core Functions
-  CreateOffsetDescriptor(\_:\_:) 

Function

# CreateOffsetDescriptor(\_:\_:)

Creates an offset descriptor that specifies the position of an element in relation to the beginning or end of its container.

macOS 10.0+

``` source
func CreateOffsetDescriptor(
    _ theOffset: Int,
    _ theDescriptor: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theOffset`  

A positive integer that specifies the offset from the beginning of the container (the first element has an offset of 1), or a negative integer that specifies the offset from the end (the last element has an offset of –1).

`theDescriptor`  

A pointer to a descriptor. On successful return, the offset descriptor created by `CreateOffsetDescriptor`. On error, returns a null descriptor. Your application must dispose of the descriptor after it has finished using it. See AEDesc.

## Return Value

A result code. See Result Codes.

## See Also

### Creating Object Specifiers

func CreateCompDescriptor(DescType, UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a comparison descriptor that specifies how to compare one or more Apple event objects with either another Apple event object or a descriptor.

func CreateLogicalDescriptor(UnsafeMutablePointer&lt;AEDescList>!, DescType, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a logical descriptor that specifies a logical operator and one or more logical terms for the Apple Event Manager to evaluate.

func CreateObjSpecifier(DescType, UnsafeMutablePointer&lt;AEDesc>!, DescType, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Assembles an object specifier that identifies one or more Apple event objects, from other descriptors.

func CreateRangeDescriptor(UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a range descriptor that specifies a series of consecutive elements in the same container.

