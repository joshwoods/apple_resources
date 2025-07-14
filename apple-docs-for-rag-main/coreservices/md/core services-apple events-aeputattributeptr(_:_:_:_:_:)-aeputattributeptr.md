

- Core Services
- Apple Events
-  AEPutAttributePtr(\_:\_:\_:\_:\_:) 

Function

# AEPutAttributePtr(\_:\_:\_:\_:\_:)

Adds a pointer to data, a descriptor type, and a keyword to an Apple event as an attribute.

macOS 10.0+

``` source
func AEPutAttributePtr(
    _ theAppleEvent: UnsafeMutablePointer!,
    _ theAEKeyword: AEKeyword,
    _ typeCode: DescType,
    _ dataPtr: UnsafeRawPointer!,
    _ dataSize: Size
) -> OSErr
```

## Parameters 

`theAppleEvent`  

A pointer to the Apple event to add an attribute to. See the AppleEvent data type.

`theAEKeyword`  

The keyword for the attribute to add. If the Apple event already includes an attribute with this keyword, the attribute is replaced.

Some keyword constants are described in Keyword Attribute Constants.

See AEKeyword.

`typeCode`  

The descriptor type for the attribute to add. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`dataPtr`  

A pointer to the data for the attribute to add.

`dataSize`  

The length, in bytes, of the data for the attribute to add.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

## See Also

### Adding Parameters and Attributes to Apple Events and Apple Event Records

func AEPutAttributeDesc(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, UnsafePointer&lt;AEDesc>!) -> OSErr

Adds a descriptor and a keyword to an Apple event as an attribute.

func AEPutParamDesc(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, UnsafePointer&lt;AEDesc>!) -> OSErr

Inserts a descriptor and a keyword into an Apple event or Apple event record as an Apple event parameter.

func AEPutParamPtr(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSErr

Inserts data, a descriptor type, and a keyword into an Apple event or Apple event record as an Apple event parameter.

