

- Core Services
- Apple Events
-  AEGetNthDesc(\_:\_:\_:\_:\_:) 

Function

# AEGetNthDesc(\_:\_:\_:\_:\_:)

Copies a descriptor from a specified position in a descriptor list into a specified descriptor; typically used when your application needs to pass the extracted data to another function as a descriptor.

macOS 10.0+

``` source
func AEGetNthDesc(
    _ theAEDescList: UnsafePointer!,
    _ index: Int,
    _ desiredType: DescType,
    _ theAEKeyword: UnsafeMutablePointer!,
    _ result: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theAEDescList`  

A pointer to the descriptor list to get the descriptor from. See AEDescList.

`index`  

A one-based positive integer indicating the position of the descriptor to get. `AEGetNthDesc` returns an error if you pass zero, a negative number, or a value that is out of range.

`desiredType`  

The desired descriptor type for the descriptor to copy. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants.

If the descriptor specified by the `index` parameter is not of the desired type, `AEGetNthDesc` attempts to coerce it to this type. However, if you pass a value of `typeWildCard`, no coercion is performed, and the descriptor type of the copied descriptor is the same as the descriptor type of the original descriptor.

See DescType.

`theAEKeyword`  

A pointer to a keyword. On successful return, the keyword for the specified descriptor, if you are getting data from a list of keyword-specified descriptors; otherwise, `AEGetNthDesc` returns the value `typeWildCard`. Some keyword constants are described in Keyword Attribute Constants and Keyword Parameter Constants. See AEKeyword.

`result`  

A pointer to a descriptor. On successful return, a copy of the descriptor specified by the `index` parameter, coerced, if necessary, to the descriptor type specified by the `desiredType` parameter. On error, a null descriptor. If the function returns successfully, your application should call the AEDisposeDesc(_:) function to dispose of the resulting descriptor after it has finished using it. See AEDesc.

## Return Value

A result code. See Result Codes.

## Discussion

If the Nth descriptor in the list is itself an Apple event record and the desired type is not wildcard, record, or list, `AEGetNthDesc` will fail with an `errAECoercionFailed` error. This behavior prevents coercion problems.

You may find the AEGetNthPtr(_:_:_:_:_:_:_:_:) function convenient for retrieving data for direct use in your application, as it includes automatic coercion.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Getting Items From Descriptor Lists

func AEGetArray(UnsafePointer&lt;AEDescList>!, AEArrayType, AEArrayDataPointer!, Size, UnsafeMutablePointer&lt;DescType>!, UnsafeMutablePointer&lt;Size>!, UnsafeMutablePointer&lt;Int>!) -> OSErr

Extracts data from an Apple event array created with the `AEPutArray` function and stores it as a standard array of fixed size items in the specified buffer.

func AEGetNthPtr(UnsafePointer&lt;AEDescList>!, Int, DescType, UnsafeMutablePointer&lt;AEKeyword>!, UnsafeMutablePointer&lt;DescType>!, UnsafeMutableRawPointer!, Size, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets a copy of the data from a descriptor at a specified position in a descriptor list; typically used when your application needs to work with the extracted data directly.

