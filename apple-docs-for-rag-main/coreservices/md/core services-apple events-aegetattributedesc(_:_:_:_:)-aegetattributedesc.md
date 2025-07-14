

- Core Services
- Apple Events
-  AEGetAttributeDesc(\_:\_:\_:\_:) 

Function

# AEGetAttributeDesc(\_:\_:\_:\_:)

Gets a copy of the descriptor for a specified Apple event attribute from an Apple event; typically used when your application needs to pass the descriptor on to another function.

macOS 10.0+

``` source
func AEGetAttributeDesc(
    _ theAppleEvent: UnsafePointer!,
    _ theAEKeyword: AEKeyword,
    _ desiredType: DescType,
    _ result: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theAppleEvent`  

A pointer to the Apple event to get the attribute descriptor from. See AppleEvent.

`theAEKeyword`  

The keyword that specifies the desired attribute. Some keyword constants are described in Keyword Attribute Constants. See AEKeyword.

`result`  

A pointer to a descriptor. On successful return, a copy of the specified Apple event attribute, coerced, if necessary, to the descriptor type specified in `desiredType`. On error, a null descriptor. If the function returns successfully, your application should call the AEDisposeDesc(_:) function to dispose of the resulting descriptor after it has finished using it. See AEDesc.

## Return Value

A result code. See Result Codes.

## Discussion

To get Apple event attribute data for your application to use directly, call AEGetAttributePtr(_:_:_:_:_:_:_:). To get a descriptor for an Apple event attribute to pass on to another Apple Event Manager routine, call `AEGetAttributeDesc`.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Getting Data or Descriptors From Apple Events and Apple Event Records

func AEGetAttributePtr(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;DescType>!, UnsafeMutableRawPointer!, Size, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets a copy of the data for a specified Apple event attribute from an Apple event; typically used when your application needs to work with the data directly.

func AEGetParamDesc(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Gets a copy of the descriptor for a keyword-specified Apple event parameter from an Apple event or an Apple event record.

func AEGetParamPtr(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;DescType>!, UnsafeMutableRawPointer!, Size, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets a copy of the data for a specified Apple event parameter from an Apple event or an Apple event record.

