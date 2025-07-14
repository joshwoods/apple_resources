

- Core Services
- Apple Events
-  AEGetAttributePtr(\_:\_:\_:\_:\_:\_:\_:) 

Function

# AEGetAttributePtr(\_:\_:\_:\_:\_:\_:\_:)

Gets a copy of the data for a specified Apple event attribute from an Apple event; typically used when your application needs to work with the data directly.

macOS 10.0+

``` source
func AEGetAttributePtr(
    _ theAppleEvent: UnsafePointer!,
    _ theAEKeyword: AEKeyword,
    _ desiredType: DescType,
    _ typeCode: UnsafeMutablePointer!,
    _ dataPtr: UnsafeMutableRawPointer!,
    _ maximumSize: Size,
    _ actualSize: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theAppleEvent`  

A pointer to the Apple event to get the attribute data from. See AppleEvent.

`theAEKeyword`  

The keyword that specifies the desired attribute. Some keyword constants are described in Keyword Attribute Constants. See AEKeyword.

`desiredType`  

The desired descriptor type for the copied data. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants.

If the descriptor specified by the `theAEKeyword` parameter is not of the desired type, `AEGetAttributePtr` attempts to coerce the data to this type. However, if you pass a value of `typeWildCard`, no coercion is performed, and the descriptor type of the returned data is the same as the descriptor type of the Apple event attribute.

On return, you can determine the actual descriptor type by examining the `typeCode` parameter.

See DescType.

`typeCode`  

A pointer to a descriptor type. On return, specifies the descriptor type of the attribute data pointed to by `dataPtr`. The returned type is either the same as the type specified by the `desiredType` parameter or, if the desired type was type wildcard, the true type of the descriptor. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`dataPtr`  

A pointer to a buffer, local variable, or other storage location, created and disposed of by your application. The size in bytes must be at least as large as the value you pass in the `maximumSize` parameter. On return, contains the attribute data.

`maximumSize`  

The maximum length, in bytes, of the expected attribute data. The `AEGetAttributePtr` function will not return more data than you specify in this parameter.

`actualSize`  

A pointer to a size variable. On return, the length, in bytes, of the data for the specified Apple event attribute. If this value is larger than the value you passed in the `maximumSize` parameter, the buffer pointed to by `dataPtr` was not large enough to contain all of the data for the attribute, though `AEGetAttributePtr` does not write beyond the end of the buffer. If the buffer was too small, you can resize it and call `AEGetAttributePtr` again.

## Return Value

A result code. See Result Codes.

## Discussion

To get Apple event attribute data for your application to use directly, call `AEGetAttributePtr`. To get a descriptor for an Apple event attribute to pass on to another Apple Event Manager routine, call AEGetAttributeDesc(_:_:_:_:).

Before calling `AEGetAttributePtr`, you can call the AESizeOfAttribute(_:_:_:_:) function to determine a size for the `dataPtr` buffer. However, unless you specify `typeWildCard` for the `desiredType` parameter, `AEGetAttributePtr` may coerce the data, which may cause the size of the data to change.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Getting Data or Descriptors From Apple Events and Apple Event Records

func AEGetAttributeDesc(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Gets a copy of the descriptor for a specified Apple event attribute from an Apple event; typically used when your application needs to pass the descriptor on to another function.

func AEGetParamDesc(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Gets a copy of the descriptor for a keyword-specified Apple event parameter from an Apple event or an Apple event record.

func AEGetParamPtr(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;DescType>!, UnsafeMutableRawPointer!, Size, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets a copy of the data for a specified Apple event parameter from an Apple event or an Apple event record.

