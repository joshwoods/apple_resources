

- Core Services
- Apple Events
-  AEPutDesc(\_:\_:\_:) 

Function

# AEPutDesc(\_:\_:\_:)

Adds a descriptor to any descriptor list, possibly replacing an existing descriptor in the list.

macOS 10.0+

``` source
func AEPutDesc(
    _ theAEDescList: UnsafeMutablePointer!,
    _ index: Int,
    _ theAEDesc: UnsafePointer!
) -> OSErr
```

## Parameters 

`theAEDescList`  

A pointer to the descriptor list to add a descriptor to. See AEDescList.

`index`  

A one-based positive integer indicating the position to insert the descriptor at. If there is already a descriptor in the specified position, it is replaced.

You can pass a value of zero or count + 1 to add the descriptor at the end of the list. `AEPutDesc` returns an error (`AEIllegalIndex`) if you pass a negative number or a value that is out of range.

`theAEDesc`  

A pointer to the descriptor to add to the list. See AEDesc.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

## See Also

### Adding Items to Descriptor Lists

func AEPutArray(UnsafeMutablePointer&lt;AEDescList>!, AEArrayType, UnsafePointer&lt;AEArrayData>!, DescType, Size, Int) -> OSErr

Inserts the data for an Apple event array into a descriptor list, replacing any previous descriptors in the list.

func AEPutPtr(UnsafeMutablePointer&lt;AEDescList>!, Int, DescType, UnsafeRawPointer!, Size) -> OSErr

Inserts data specified in a buffer into a descriptor list as a descriptor, possibly replacing an existing descriptor in the list.

