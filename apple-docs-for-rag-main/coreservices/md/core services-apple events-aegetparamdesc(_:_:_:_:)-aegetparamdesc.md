

- Core Services
- Apple Events
-  AEGetParamDesc(\_:\_:\_:\_:) 

Function

# AEGetParamDesc(\_:\_:\_:\_:)

Gets a copy of the descriptor for a keyword-specified Apple event parameter from an Apple event or an Apple event record.

macOS 10.0+

``` source
func AEGetParamDesc(
    _ theAppleEvent: UnsafePointer!,
    _ theAEKeyword: AEKeyword,
    _ desiredType: DescType,
    _ result: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theAppleEvent`  

A pointer to the Apple event to get the parameter descriptor from.

`theAEKeyword`  

A keyword that specifies the desired Apple event parameter. Some keyword constants are described in Keyword Parameter Constants.

`desiredType`  

The descriptor type for the desired Apple event parameter. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants.

If the requested Apple event parameter is not of the desired type, the Apple Event Manager attempts to coerce it to the desired type. However, if you pass a value of `typeWildCard`, no coercion is performed, and the descriptor type of the returned descriptor is the same as the descriptor type of the Apple event parameter.

`result`  

A pointer to a descriptor. On successful return, a copy of the descriptor for the specified Apple event parameter, coerced, if necessary, to the descriptor type specified by the `desiredType` parameter. On error, a null descriptor. If the function returns successfully, your application should call the AEDisposeDesc(_:) function to dispose of the resulting descriptor after it has finished using it.

## Return Value

A result code. See Result Codes.

## Discussion

You typically call `AEGetParamDesc` to get a descriptor for an Apple event parameter to pass on to another Apple Event Manager routine. To get Apple event parameter data for your application to use directly, call AEGetParamPtr(_:_:_:_:_:_:_:).

If the actual parameter you are getting with `AEGetParamDesc` is a record, you can only request it as a `typeAERecord`, `typeAEList`, or `typeWildcard`. For any other type, `AEGetParamDesc` will return `errAECoercionFail`.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Getting Data or Descriptors From Apple Events and Apple Event Records

func AEGetAttributeDesc(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Gets a copy of the descriptor for a specified Apple event attribute from an Apple event; typically used when your application needs to pass the descriptor on to another function.

func AEGetAttributePtr(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;DescType>!, UnsafeMutableRawPointer!, Size, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets a copy of the data for a specified Apple event attribute from an Apple event; typically used when your application needs to work with the data directly.

func AEGetParamPtr(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;DescType>!, UnsafeMutableRawPointer!, Size, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets a copy of the data for a specified Apple event parameter from an Apple event or an Apple event record.

