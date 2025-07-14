

- Core Services
- Apple Events
-  AEPutParamPtr(\_:\_:\_:\_:\_:) 

Function

# AEPutParamPtr(\_:\_:\_:\_:\_:)

Inserts data, a descriptor type, and a keyword into an Apple event or Apple event record as an Apple event parameter.

macOS 10.0+

``` source
func AEPutParamPtr(
    _ theAppleEvent: UnsafeMutablePointer!,
    _ theAEKeyword: AEKeyword,
    _ typeCode: DescType,
    _ dataPtr: UnsafeRawPointer!,
    _ dataSize: Size
) -> OSErr
```

## Parameters 

`theAppleEvent`  

A pointer to the Apple event to add a parameter to. See the AppleEvent data type.

`theAEKeyword`  

The keyword for the parameter to add. If the Apple event already includes an parameter with this keyword, the parameter is replaced.

Some keyword constants are described in Keyword Parameter Constants.

See AEKeyword.

`typeCode`  

The descriptor type for the parameter to add. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`dataPtr`  

A pointer to the data for the parameter to add.

`dataSize`  

The length, in bytes, of the data for the parameter to add.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

## See Also

### Adding Parameters and Attributes to Apple Events and Apple Event Records

func AEPutAttributeDesc(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, UnsafePointer&lt;AEDesc>!) -> OSErr

Adds a descriptor and a keyword to an Apple event as an attribute.

func AEPutAttributePtr(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSErr

Adds a pointer to data, a descriptor type, and a keyword to an Apple event as an attribute.

func AEPutParamDesc(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, UnsafePointer&lt;AEDesc>!) -> OSErr

Inserts a descriptor and a keyword into an Apple event or Apple event record as an Apple event parameter.

