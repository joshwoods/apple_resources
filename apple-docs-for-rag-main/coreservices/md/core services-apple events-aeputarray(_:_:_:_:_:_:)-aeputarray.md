

- Core Services
- Apple Events
-  AEPutArray(\_:\_:\_:\_:\_:\_:) 

Function

# AEPutArray(\_:\_:\_:\_:\_:\_:)

Inserts the data for an Apple event array into a descriptor list, replacing any previous descriptors in the list.

macOS 10.0+

``` source
func AEPutArray(
    _ theAEDescList: UnsafeMutablePointer!,
    _ arrayType: AEArrayType,
    _ arrayPtr: UnsafePointer!,
    _ itemType: DescType,
    _ itemSize: Size,
    _ itemCount: Int
) -> OSErr
```

## Parameters 

`theAEDescList`  

A pointer to the descriptor list to put the Apple event array into. If there are any descriptors already in the descriptor list, they are replaced. If the array type is `kAEKeyDescArray`, `theAEDescList` must point to an Apple event record; otherwise, it can point to either a descriptor list or an Apple event record.

If you pass a pointer to a factored descriptor list, created by calling the AECreateList(_:_:_:_:) function, each array item in the array pointed to by the `arrayPtr` parameter must include the data that is common to all the descriptors in the list. The Apple Event Manager automatically isolates the common data you specified in the call to `AECreateList`. A factored descriptor list is described in the Discussion section.

See AEDescList.

`arrayType`  

The Apple event array type to create. Pass a value specified by one of the constants described in Data Array Constants. See AEArrayType.

`arrayPtr`  

A pointer to a buffer, local variable, or other storage location, created and disposed of by your application, that contains the array to put into the descriptor list. See AEArrayData.

`itemType`  

For arrays of type `kAEDataArray`, `kAEPackedArray`, or `kAEHandleArray`, the descriptor type of the array items to create. Use one of the constants described in Descriptor Type Constants, such as `typeLongInteger`. You don’t need to specify an item type for arrays of type `kAEDescArray` or `kAEKeyDescArray` because the data is already stored in descriptors which contain a descriptor type. See DescType.

`itemSize`  

For arrays of type `kAEDataArray` or `kAEPackedArray`, the size (in bytes) of the array items to create. You don’t need to specify an item size for arrays of type `kAEDescArray`, `kAEKeyDescArray`, or `kAEHandleArray` because their descriptors (though not the data they point to) have a known size.

`itemCount`  

The number of elements in the array.

## Return Value

A result code. See Result Codes.

## Discussion

A factored descriptor list is one in which the Apple Event Manager automatically isolates the data that is common to all the elements of the list so that the common data only appears in the list once. To create a factored descriptor list, you call the AECreateList(_:_:_:_:) function and specify the data that is common to all elements in the descriptor array.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Adding Items to Descriptor Lists

func AEPutDesc(UnsafeMutablePointer&lt;AEDescList>!, Int, UnsafePointer&lt;AEDesc>!) -> OSErr

Adds a descriptor to any descriptor list, possibly replacing an existing descriptor in the list.

func AEPutPtr(UnsafeMutablePointer&lt;AEDescList>!, Int, DescType, UnsafeRawPointer!, Size) -> OSErr

Inserts data specified in a buffer into a descriptor list as a descriptor, possibly replacing an existing descriptor in the list.

