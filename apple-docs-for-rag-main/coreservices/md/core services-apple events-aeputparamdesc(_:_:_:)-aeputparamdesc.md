

- Core Services
- Apple Events
-  AEPutParamDesc(\_:\_:\_:) 

Function

# AEPutParamDesc(\_:\_:\_:)

Inserts a descriptor and a keyword into an Apple event or Apple event record as an Apple event parameter.

macOS 10.0+

``` source
func AEPutParamDesc(
    _ theAppleEvent: UnsafeMutablePointer!,
    _ theAEKeyword: AEKeyword,
    _ theAEDesc: UnsafePointer!
) -> OSErr
```

## Parameters 

`theAppleEvent`  

A pointer to the Apple event to add a parameter to. See the AppleEvent data type.

`theAEKeyword`  

The keyword specifying the parameter to add. If the Apple event already has a parameter with this keyword, the parameter is replaced.

Some keyword constants are described in Keyword Parameter Constants.

See AEKeyword.

`theAEDesc`  

A pointer to the descriptor for the parameter to add. See AEDesc.

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

func AEPutParamPtr(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSErr

Inserts data, a descriptor type, and a keyword into an Apple event or Apple event record as an Apple event parameter.

