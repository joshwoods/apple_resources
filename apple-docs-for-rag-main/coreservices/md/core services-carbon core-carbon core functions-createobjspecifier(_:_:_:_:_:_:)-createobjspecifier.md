

- Core Services
- Carbon Core
- Carbon Core Functions
-  CreateObjSpecifier(\_:\_:\_:\_:\_:\_:) 

Function

# CreateObjSpecifier(\_:\_:\_:\_:\_:\_:)

Assembles an object specifier that identifies one or more Apple event objects, from other descriptors.

macOS 10.0+

``` source
func CreateObjSpecifier(
    _ desiredClass: DescType,
    _ theContainer: UnsafeMutablePointer!,
    _ keyForm: DescType,
    _ keyData: UnsafeMutablePointer!,
    _ disposeInputs: Bool,
    _ objSpecifier: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`desiredClass`  

The object class of the desired Apple event objects. See DescType.

`theContainer`  

A pointer to a descriptor that describes the container for the requested object, usually in the form of another object specifier. See AEDesc.

`keyForm`  

The key form for the object specifier.

`keyData`  

A pointer to a descriptor that supplies the key data for the object specifier.

`disposeInputs`  

A Boolean value. Pass (`TRUE`) if the function should dispose of the descriptors for the `theContainer` and `keyData` parameters or (`FALSE`) if your application will. A value of `FALSE` may be more efficient for some applications because it allows them to reuse descriptors.

`objSpecifier`  

On successful return, a pointer to the object specifier created by the `CreateObjSpecifier` function. If the function returns successfully, your application should call the AEDisposeDesc(_:) function to dispose of this descriptor after it has finished using it.

## Return Value

A result code. See Result Codes.

## See Also

### Creating Object Specifiers

func CreateCompDescriptor(DescType, UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a comparison descriptor that specifies how to compare one or more Apple event objects with either another Apple event object or a descriptor.

func CreateLogicalDescriptor(UnsafeMutablePointer&lt;AEDescList>!, DescType, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a logical descriptor that specifies a logical operator and one or more logical terms for the Apple Event Manager to evaluate.

func CreateOffsetDescriptor(Int, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates an offset descriptor that specifies the position of an element in relation to the beginning or end of its container.

func CreateRangeDescriptor(UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a range descriptor that specifies a series of consecutive elements in the same container.

