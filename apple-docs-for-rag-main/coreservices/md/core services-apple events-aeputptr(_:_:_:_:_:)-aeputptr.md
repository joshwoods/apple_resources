

- Core Services
- Apple Events
-  AEPutPtr(\_:\_:\_:\_:\_:) 

Function

# AEPutPtr(\_:\_:\_:\_:\_:)

Inserts data specified in a buffer into a descriptor list as a descriptor, possibly replacing an existing descriptor in the list.

macOS 10.0+

``` source
func AEPutPtr(
    _ theAEDescList: UnsafeMutablePointer!,
    _ index: Int,
    _ typeCode: DescType,
    _ dataPtr: UnsafeRawPointer!,
    _ dataSize: Size
) -> OSErr
```

## Parameters 

`theAEDescList`  

A pointer to the descriptor list to add a descriptor to. See AEDescList.

`index`  

A one-based positive integer indicating the position to insert the descriptor at. If there is already a descriptor in the specified position, it is replaced.

You can pass a value of zero or count + 1 to add the descriptor at the end of the list. `AEPutPtr` returns an error (`AEIllegalIndex`) if you pass a negative number or a value that is out of range.

`typeCode`  

The descriptor type for the descriptor to be put into the list. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`dataPtr`  

A pointer to the data for the descriptor to add.

`dataSize`  

The length, in bytes, of the data for the descriptor to add.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

## See Also

### Adding Items to Descriptor Lists

func AEPutArray(UnsafeMutablePointer&lt;AEDescList>!, AEArrayType, UnsafePointer&lt;AEArrayData>!, DescType, Size, Int) -> OSErr

Inserts the data for an Apple event array into a descriptor list, replacing any previous descriptors in the list.

func AEPutDesc(UnsafeMutablePointer&lt;AEDescList>!, Int, UnsafePointer&lt;AEDesc>!) -> OSErr

Adds a descriptor to any descriptor list, possibly replacing an existing descriptor in the list.

